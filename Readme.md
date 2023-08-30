## create the table
```
CREATE TABLE IF NOT EXISTS `product_option_recurring_mapping` (
    `mapping_id` INT(11) NOT NULL AUTO_INCREMENT,
    `product_id` INT(11) NOT NULL,
    `option_value_id` INT(11) NOT NULL,
    `recurring_id` INT(11) NOT NULL,
    PRIMARY KEY (`mapping_id`),
    UNIQUE KEY `product_option` (`product_id`,`option_value_id`)
) 
ENGINE=MyISAM DEFAULT CHARSET=utf8 AUTO_INCREMENT=1;
```
# Regex

The RegEx used in the CreditCardValidation function is either for the format of credit card numbers for Mastercard or Visa.

For Visa cards, the regex pattern is /^4[0-9]{12}(?:[0-9]{3})?$/.

The pattern starts with a "4" to match Visa card prefix. Then it looks for 12 digits. An optional group (?:[0-9]{3}) matches the last three digits of Visa cards that have a four digit account number extension. For Mastercard, the pattern is /^(?:5[1-5][0-9]{2}|222[1-9]|22[3-9][0-9]|2[3-6][0-9]{2}|27[01][0-9]|2720)[0-9]{12}$/

The first part of the regex matches a prefix of 51 through 55
The second part matches the prefix 2221 through 2229
The third part matches the prefix 223 through 229
The fourth part matches the prefix 23 through 26
The fifth part matches the prefix 270 through 271
The sixth part matches the prefix 2720
The last part matches the next 12 digits of the card.

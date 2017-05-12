# useful-codes
Useful Codes to replicate



    @api.one
    @api.constrains('total','sr_limit')
    def _check_total(self):
        if int(self.claim_amount) > int(self.sr_limit):
            raise ValidationError('Amount is exceeding monthly limit')


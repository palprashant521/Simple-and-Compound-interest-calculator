# Simple-and-Compound-interest-calculator

class Interest:
    
    def __init__(self,p,r,t):
        
        self.p = p
        self.r = r
        self.t = t
        
    def simple_interest(self):
        
        SI = self.p*self.r*self.t/100
        si_amount = self.p + SI
        
        print("The Principle = {} \nThe rate of interest = {} \nThe time in years = {}".format(self.p,self.r,self.t))
        print('\n')
        print("The simple interest is: {}".format(SI))
        print("The Total amount = {}".format(si_amount))
        
    def compound_interest(self):
        
        CI = self.p*(1+(self.r/100))**self.t - self.p
        ci_amount = CI + self.p
        
        print("The Principle = {} \nThe rate of interest = {} \nThe time in years = {}".format(self.p,self.r,self.t))
        print('\n')
        print("The compound interest is: {}".format(CI))
        print("The Total amount = {}".format(ci_amount))
        
        

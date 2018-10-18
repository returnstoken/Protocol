## TOKENIZED REAL ESTATE MARKETPLACE

#### RealtyReturns 
#### Whitepaper v 3 9.18.18


### Introduction
Real estate is widely regarded as the best way to grow and preserve wealth, with minimal risk and a high upside. Real estate investing has not changed very much over the years. Today we are seeing everything change with blockchain technology and cryptocurrency as it disrupts the 217 trillion dollar global real estate market for the first time in history. Smart contracts and security tokens provide greater access for investors, investment transparency and security, as well as real estate liquidity on a global scale. Thus solving cross-border investing difficulties and financial restrictions creating a truly liquid real estate market.

RealtyReturns is an Ethereum based, smart contracts governed marketplace thatutilizes security tokens to provide income-producing real estate investments to investors around globe. The decentralized financial system of cryptocurrency provides a powerful instrument for investors to easily secure their capital in American real estate through our two-sided marketplace platform.


### Background

Every few years we see technology disrupt an entire industry. Most recently the real estate investing industry has been disrupted by the following trends:

Online MLS – This enables real estate investors to view properties that are available for sale from anywhere online. However, an investor has to purchase the entire property and manage it themselves.

Real Estate CrowdFunding – Online platforms enabled investors to co-own real estate or as little as $5,000. This reduced some financial limitations and property management issues, such as tenants, toilets, and maintenance.

Despite these disruptions, “traditional” real estate crowdfunding platforms such as RealtyShares and RealtyMogul are still plagued by significant issues such as; cross-border investing difficulties, financial restrictions and lack of investment liquidity. International investors are still required to have access to a U.S. bank account and their money is tied up in the property for an indefinite period of time before they are able to liquidate their investment.


### The Problems

Problem: International investors want to enter the American real estate market but
cross-border investing restrictions make it nearly impossible for them to do so.

Problem: Cryptocurrency owners seek alternative ways to receive stable income and
secure their crypto value without the constant fluctuations in the crypto markets.

Problem: Many potential investors are turned away from real estate because of the long hold periods and inability to quickly sell their investment. They do not want their money tied up for extended periods of time.
RealtyReturns White Paper		


### The Solutions

Solution: RealtyReturns’ smart contracts and security tokens solve cross-border investing restrictions, allowing investors from all over the world to easily participate in the booming American real estate market.

Solution: Our security tokens (Returns Token) represent an investors ownership stake in a specific income producing property. This provides the owner both a stable source income of income from the property as well as a shelter from the instability of the traditional cryptocurrency markets.

Solution: Since our security tokens (Returns Token) represent physical ownership in a specific property, the owner can sell their token on a security token exchange, like OpenFinance, thus creating a truly liquid real estate market.


### Business Model

RealtyReturns has a straightforward and scalable business model. We have implemented a proven model, traditional real estate crowdfunding, and improved upon it by incorporating blockchain smart contracts and security tokens. Simply put, when a buyer invests in a property by purchasing a Returns Token they receive income generated by the property and RealtyReturns earns 3% of the security token issuance.


### Smart Contract

Wheneverincomeisgeneratedby an investor’sspecificproperty, thereturns are automatically
transferred to the token holder’s ethereum wallet via smart contract.

In recent years, Turing-complete programming languages have been implemented into decentralized blockchains. These systems use smart contracts (software programs stored on the blockchain that are automatically implemented upon specific conditions being satisfied) to add and modify data random sequences based on user design.


### Tokens

RealtyReturns will issue two types of tokens:

Access Token: These are membership (utility) tokens that are required to access and invest on the RealtyReturns platform. They are used to cover all investment costs and fees such as: KYC (Know Your Customer) / AML (Anti-Money Laundering) verification checks, LLC formation and management costs, legal expenses...etc.

Returns Token: This ERC-20 security token will be backed by a specific income generating investment property. Each Returns Token is connected to a specific property via smart contract and can be sold on a security token exchange for liquidity. When income is generated by the property, the income payments are transferred directly to the token holders Ethereum wallet.


### Access Token

Access Tokens functionasmembership(utility) tokens forthe RealtyReturns.complatformandenable token holders to invest through the platform. Access Tokens are used to cover all operational costs and platform fees such as: KYC (Know Your Customer) / AML (Anti-Money Laundering) verification checks, LLC formation and management costs, legal expenses...etc.. Each unique Access Token is linked directly to the same Ethereum wallet as a specific Returns Token (see “Returns Token” below).

Duringourpre-ICO/ICOwewillbeissuing Limited-Edition ERC-20 Access Tokens toourearly supporters. These Limited-Edition Access Tokens provide token holders dividend payments without being subject to any transaction fees (i.e., 0% fee). These Access Tokens can be soldortransferred toothermembers.


### Returns Token

The Returns Token is an ERC-20 security token that represents an investors ownership stake in a specific property. The Returns Token also enables the owner (investor) to receive the income generated by that property. Each Returns Token is tied to the investors Ethereum wallet via smart contract and must be held in the same wallet as the correlating Access Token. Income payments are paid out in Ethereum and are based on the cash flows associated with the property.

Our model employs our proprietary protocol to enforce compliance on secondary transfers. The Returns Token embeds compliance at the token level and allows for decentralized trading of private securities across any platform that supports ERC-20 tokens. This significantly increases liquidity in comparison to confining trading within a single centralized exchange in order to enforce regulatory compliance. Centralized exchanges can enforce regulatory requirements to a limited degree, including KYC, AML, and accreditation.

To date, security token issuers have been unable to adequately enforce core securities regulations such as limiting the numbers of investors and stipulating ownership levels.

Our proposed solution enforces regulatory compliance at the token level, thereby
meeting core securities requirements regardless of whether the trade occurs on centralized or decentralized exchanges.

The Returns Token Standard incorporates three core services on the Ethereum blockchain:

The Returns Token
The Governor Service
The Service Recorder

We will implement all of these services as three distinct smart contracts. Implementation as
distinct smart contracts allows for easier upgrades as regulatory requirements evolve over time.


### Returns Token Tech Overview

The Returns Token is a permissioned ERC-20 smart contract that represents ownership of a specific real estate security. This ERC-20 token is compatible with all existing wallets and exchanges that support the ERC-20 token standard, however it will override the existing ERC-20 transfer method to check with an on-chain regulator service for trade approval.
Every time a transfer is initiated (e.g., John wants to transfer a token to Rob), The Returns Token calls the GovernorService#check () method from within the transfer ()2 and transferFrom ()3 methods specified in ERC-20. If the check is successful, the transfer proceeds normally per the ERC-20 specifications (i.e., the token is transferred from John to Rob). In addition, the transfer () and transferFrom () methods deliver a successful CheckStatus event.

If the check is unsuccessful, then the transfer () and transferFrom () method returns an error code (i.e., the transfer from John to Rob fails) and delivers an unsuccessful CheckStatus event with a reason code. The CheckStatus event can be used by third party wallet providers to indicate the reason why a trade was not allowed.
In the case where a mediator is required for the transfer of tokens (e.g. in a decentralized exchange), the approve ()4 Method is called to allocate funds from the token holder (e.g. Rob) to the mediator. Once allocated, the mediator initiates the transfer sequence as in Figure 2 below.
Note: The approve () method can be implemented to include an additional check () method. This would mean that the allocation of funds from the token holder  to the mediator would require approval from the Governor Service. The initial implementation of The Returns Token will not include this additional check. .
https://github.com/ethereum/EIPs/blob/master/EIPS/eip-20.md
https://github.com/ethereum/EIPs/blob/master/EIPS/eip-20.md#transfer-1
https://github.com/ethereum/EIPs/blob/master/EIPS/eip-20.md#transferfrom
https://github.com/ethereum/EIPs/blob/master/EIPS/eip-20.md#approve


### Governor Service

The Governor Service interface consists of a single check () method that is called from within the transfer () and transferFrom () method. This check contains all information provided during the transfer.

Contract GovernorService {
function check (address _token,
address_spender, address_from, address_to,
uint256 _amount) public returns (uint8) ;
}


In order to provide the Returns Token smart contract with trade approval (or disapproval), the Governor Service must include a whitelist of approved investors, their trading permissions and additional token trading settings such that it satisfies relevant securities regulations, KYC policies, AML requirements, tax laws, etc.

The first implementation of the Governor service includes two participant-level permissions and two token-level settings. Theses permissions and setting can be used to meet commonly required trading rules for private securities within a single jurisdiction.

The two participant-level permissions are 1) the permission to send a token, and 2) the permission to receive a token. Knowing the difference between send and receive permissions allows for greater flexibility. An off-chain trade controller determines

theses participant-level permissions (by reviewing the participant data they submitted such as county of residence, KYC/ AML status, tax status, accredited investor status, etc.) and writes the results to the Governor Service.

The first token-level setting in the first implementation of the governor service is locking/ unlocking transfers. This setting allows enforcement of holding periods. This is particularly important because when a token is issued under Regulation D, the buyer is confined to a one-year holding period. Our system will lock the token during this time to enforce compliance.

The second token-level setting is allowing/ disallowing partial transfers of a security token (e.g., 0.25 of a token). This setting enables capping the total number of token holders. For example, if only a maximum of 250 token holders are allowed in a certain offering, a total of 250 tokens can be issued as long as partial transfers are disallowed. In this example, to cap the token holder count to 250, a limited number of tokens can be issued to 250 participants during the initial ICO/ Token Sale.


Note: The Returns Token provides an interface that developers can use to implement custom business logic. RealtyReturns use of Governor Service will include other services not fully disclosed in this White Paper. Some of the services will be other functionalities intended to enforce multi-jurisdictional requirements at a more granular level.


### Service Recorder

The Service Recorder provides the Returns Token smart contract with a mechanism for locating the current, correct, or desired version of the Governor Service.

The Above diagram illustrates the interaction between the Returns Token, Governor Service, and Service Recorder. The service recorder provides the appropriate governor service address to Returns Token; the Returns Token then checks with the Governor Service to obtain trade approvals.

When a new version of the Governor Service is released, the service recorder provides the update Governor Service address to the Returns Token. This ensures that the correct Governor Service is used for trade approval. See below diagram.

Note: The Returns Token provides an interface that developers can use to implement custom business logic. Other implementations of service recorder could allow for multiple Governor Service to exist at once, making it possible to decentralize the Governor Service.


### Marketplace Control Room

The first implementation of the Governor Service requires an off-chain marketplace control room to update its permissions as well as add newly approved investors. RealtyReturns will initially act as the marketplace control room and will enable decentralization of this role to third party platforms in the future.

The marketplace control room determines the status of the permissions. It maps investors data against relevant securities regulations, KYC/ AML policies, and tax laws to determine whether each participant can send and/ or receive a security token. It also determines whether the token is locked/ unlocked and whether any trading is allowed or disallowed. These token-level permissions are then updated in the Governor Service.

Only the marketplace control room and team can correct private/ public key pairings or make changes to the Governor Service.


### Legal Framework For Real Estate Investment

Investors will purchase Returns Tokens that represent ownership/membership units of the LLC that holds title to the property and they will be able to hold the security tokens in their wallets or trade them via a secondary transaction to another buyer. Subject to LLC articles/bylaws, the security tokens will produce income in Ethereum which will be automatically transferred on a recurring basis to the specific wallet which holds the security token as well as the corresponding Access Token.


### Token Sale

Our maximum token supply is 1.2-Billion (1,200,000,000) Access Tokens connected via smart contract.

Up to 192-million of these Limited-Edition Access Tokens (16%) will be sold to our early
supporters via smart contract during the pre-ICO/ICO.

20% of the total Membership tokens will be created and held by the RealtyReturns Treasury (240-million).

10% will be for our advisors, influencers, team members, brand ambassadors, mass
adoption project sponsors, and incentive programs (120-million).

10% will be allocated to founders and are subject to a vesting period (120-million).

44% will be allocated for new investors and network growth (528-million), such as the live bounty campaign we recently launched with 2-Million allocated tokens (RRT).

### Token Crowd-Sale


Start Date: October 23rd, 2018.
-	100 Million	@ $0.15
-	40 Million	@ $0.30
-	40 Million	@ $0.50
-	10 Million	@ $0.80
190 Million - ICO Crowd Sale
240 Million - RealtyReturns Treasury 120 Million - Team and Advisors
120 Million - Founders
530 Million - Network Growth

Use of Proceeds
5%

30%
Blockchain and Database Development
Legal/Regulatory
Cyber Security
5%
10%
Operation and Services

10%




25%
Community,
Adoption, Marketing
First 5 Properties

15%
Front-End
Network Development
Note: All dates and amounts are estimates and may be subject to change.


### Example Real Estate Transaction

Our network is constantly reviewing cash flow positive investment properties in the United States. We have built a strong and trusting working relationship with our real estate partners nationwide. These relationships enable us to work directly alongside real estate developers, brokers, agents and owners to identify and participate in the best cash flow positive commercial and residential investment opportunities available for our investors.

Our investments are typically offered in the following arrangements:

The entire property is purchased from the current owner and is managed by our professional property management team.
RealtyReturns co-invests with trusted partners, developers, funds and family offices as
a co-owner.

Providing hard money loans to professional developers who fix and flip rehabilitation properties, earning monthly interest payments. The deed of trust / first lien position of the property is always held by RealtyReturns in these types of investments in case of any defaults by the borrower. To mitigate default risk, we only lend to trusted developers with a verifiable and proven track record.

Once we have identified an investment that meets our criteria we begin a detailed
due diligence process that ensures only the most promising real estate investment opportunities are available to our members. We place emphasis on the following areas:

The property’s cash flow history.
Investment terms. We will only participate in investment structures that favor
RealtyReturns investors.
The current owner/ operator’s track record.
If providing a hard money loan, track record is particularly important and is an main area of focus for our team. We also place emphasis on LTV (Loan to Value) of the property (+75% LTV).
The condition of the property, depreciation, rehabilitation needs (if any), past and current occupancy rates...etc.
The track record and reputation of any other parties associated with the investment.

### Whitelist

The Whitelist is like a complex waiting list and due diligence process:

After an investor joins the Whitelist for a specific investment, our vendor and RealtyReturns will do a “Know Your Customer” (KYC), “Anti-Money Laundering” (AML) and “Terrorist Check”. We will also ask them for their MyEtherWallet address and upon clearance we may ask the investor to send a test amount of Ethereum (ETH), so we can verify ownership of their MyEtherWallet address.

Once these checks have been completed and the investor is approved, they will be added to the whitelist.
Legal Setup

A specific LLC with a unique name is setup for every investment. The actual ownership interest in the investment is held by the LLC itself. Each LLC will be registered and operated in and from the United States. All investors participating in the specific investment will be partial owners, limited partners in the LLC.

Each LLC will be divided up into membership units. A membership unit represents an ownership stake in the LLC. The membership units sold will be passive/minority ownership stakes. These LLC members will receive the economic benefits of the asset, but they will not be involved in any management decisions or physical operations of the property.

### Smart Contract Setup

The smart contract will be setup so that a specific amount of Ether will be required to purchase a Returns Tokens. There will be a unique token provided for each investment. Example: “Returns Token XYZ” (“XYZ” refers to the unique identification number assigned to the investment).

Once an investor purchases a Returns Token, that token will be legally and technically connected to a membership unit of the LLC that holds the property. The LLC documents will name each individual token by referencing the unique token code for each LLC member.

In summary; each unique token will be named in the LLC documents (by membership unit
number/ token owner), and the investors will hold the tokens in their private wallets.

### Escrow Process

Investors will be provided with the smart contract address so they can send their investment to purchase the Returns Token associated with the specific investment property.

The Ether or USD will be sent directly to a 3rd party escrow company and held there until the total amount is raised. RealtyReturns has no access to the funds when they are being held by a 3rd party escrow company. Once the total amount for the investment is received, the escrow company transfers the funds to the investment destination and the investment is completed.
How Investors Get Paid

Income generated from investments will be paid out in accordance with the specific
investment terms agreed to upon the initial investment.

Equity Investments: All rental income generated by an investment property will be divided amongst the members of the LLC in accordance with the ownership percentages they hold (membership units).

Debt Investments (Lending): The developer pays recurring interest payments as defined in
their signed lending agreement.

Income generated from all investment types will be paid out directly to investors into the
MyEtherWallet address they provided in Ethereum.

All payments are recorded and visible on the Ethereum blockchain. This is important if the investor wants to sell their Returns Token to another investor because it allows the potential buyer to see the income payments, which are clearly tracked on the blockchain.
Purpose & Use of the Access Token

Income from a Returns Token will only be paid to an investor’s wallet if it also holds the corresponding Access Token. All investors and LLC members must have both a Returns Token and the specific corresponding Access Token.
RealtyReturns White Paper	

Access tokens cover all platform fees and provide investor access to invest through the platform.
Token Liquidity

If an investor wishes to sell their membership unit in an investment for liquidity, they are able to do so through through the RealtyReturns platform or a listed security token exchange.

### Future Property Sale

If an investment property is sold in the future, any gains will be distributed in Ether to the
wallets of all the Returns Token and Access Token holders for the corresponding property.
The distribution process is the same as mentioned above for income distribution.


### Team

#### Manny Fernandez, Co-Founder, CEO
Manny Fernandez is a Stanford University educated angel investor, serial entrepreneur, and best-selling author featured on CNBC’s Make Me A Millionaire Inventor. He has been successful investing in his own ideas as well as taking companies from startup to exit.

Manny is the founder of Sacramento Affordable Housing Organization, Inc. (SAHO), acquires vacant and foreclosed single-family residential properties located within specific target areas of the City and County of Sacramento that have transferred to banks or lending institutions. SAHO has been qualified and participated as a residential development partner in the federally funded Neighborhood Stabilization Program (NSP), which is managed by the Sacramento Housing and Redevelopment Agency (SHRA) and focuses on the rehabilitation and sale of foreclosed single-family homes to owner occupants. SAHO is a Neighborhood Stabilization Program sub-recipient.

SAHO was an active developer partner in the Foreclosed Property Access and Rehabilitation Program, which is administered by SHRA and operates in partnership with the federal National Community Stabilization Trust (NCST). The program is complementary to other programs under the NSP, providing access to foreclosed properties in negatively impacted areas of the City and County of Sacramento.

All of Fernandez’s experience in the investment landscape has culminated, under his leadership, in the first Silicon Valley/San Francisco based FINRA and SEC-registered funding portal DreamFunded.com.


#### Rexford R. Hibbs, Co-Founder, COO

Rexford co-founded DreamFunded.com, San Francisco’s 1st Title III equity crowdfunding platform. Rexford wanted to combine his background in real estate and his expertise in equity crowdfunding.

He is an investor from a successful real estate and angel investing background, making and managing real estate investments in Washington, Oregon, Arizona and California through his family office. Before co-founding DreamFunded, Rexford was previously on the real estate investment committee with Marcus& Millichap, working closely with brokers to procure promising investment opportunities. Rexford is a Seattle native with deep ties to the real estate investment networks in Seattle, Sacramento, the San Francisco Bay Area, Phoenix and Hawaii.

#### Alexandr Larinov, Co-Founder, CTO
Alexandr is Co-Founder and CTO at RealtyReturns. He has successfully built two crowdfunding platforms from the ground up. Bringing his wealth of experience to RealtyReturns he focuses on building the platform and he is responsible for overseeing all technical aspects of the company such as UX/UI, testing, deployment, and implementation. Alexandr brings his expertise in Ruby on Rails, Javascript and React to the team.


#### Gustavo Guimares, Blockchain/ Smart Contract Engineer
Gustavo is an  Experienced  Software Engineer  with a demonstrated history of working in the internet industry. Furthermore, he worked as a Smart Contract Engineer at Starbase.co. He is skilled in Blockchain development, Ethereum protocol, Smart contracts, Analytical Skills, Databases, JavaScript (React.js) and Ruby. Strong engineering professional graduated from Lawrence University.


#### Robert Loebl, Deal Flow Manager
Robert is a Bay Area-based commercial real estate broker who focuses his nationwide investment sales practice on net leased asset dispositions. He is a Certified Commercial Investment Member (CCIM) and has experience transacting across multiple product types, including sales and leasing of retail, medical, industrial, multifamily, and office properties. He is   a graduate with high distinction in economics and philosophy from the University of Virginia and is passionate about blockchain’s potential to disrupt the real estate industry.
Trevor Whiting, Investor Relations
Trevor was VP of Investor Relations for real estate crowdfunding company RealtyMogul.com, who is one of the leaders in traditional real estate crowdfunding. Trevor was accountable for revenue, profit, sales operations and growth initiatives. Under his leadership, he developed a sales playbook that resulted in 2x revenue growth.


#### Youdong Zhang, Software Engineer Intern
Youdong Zhang was a software engineering intern at Facebook and Google with expertise in elastic search, web development, and data analysis. Previously, Youdong was a machine learning researcher at the Berkeley Institute of Data Science and is currently researching algorithms at the Nuclear Engineering Department at the University of California, Berkeley. She was also on the original programming team that built the DreamFunded platform.


#### Vis Chen, FinTech Research
Vis has worked as an intern at Accenture Services where he provides technology consulting. He has also worked as an MBA consultant for Verizon at Cornell.


### Advisors

#### Yuguang Li, Social Media Marketing
Yuguang, handles social media marketing  in  Asia.  He Performed financial due diligence for real estate properties. He analyzes blockchain technology, tokenized business models, and was involved in creating the white paper  for  RealtyReturns’s  ICO.  He is fluent Mandarin and Cantonese.

#### Salil Pradhan, Venture Partner: Draper Nexus
Salil is a venture partner and early-stage investor at Tim Draper’s VC firm. He is an advisor to corporate LPs on product strategy, partnerships with startups, and mergers & acquisitions.

#### Joseph Huang, Infinity Ventures Managing Partner Joseph  is  an  investment  partner  at  Infinity  Venture
Partners, dabbling in the seed round and the A round investment of Internet, mobile industry, software, digital content industry, and disruptive technology. Prior to the Infinity Ventures, he was an investment partner at Abico VC and co-founder of Gamesamba.

#### Bob Hibbs, Esp, Real Estate Developer
Mr. Hibbs is active and well known in West Coast real estate circles providing legal representation for owners and for lenders, and currently as an owner/developer for his family office. He has worked for the last 20 years on some of the Pacific Northwest’s, Oregon’s and Arizona’s premier real estate projects. Mr. Hibbs now devotes his time toward real estate projects for his family office.

#### John Rampton, Public Relations
John   helped   launch   IOTA,   the   10th   most   traded token  on  CoinMarketCap.com.  John  was  named  #2 on Entrepreneur Magazine’s list of Top 50 Online Influencers in the World. He is also a blogging expert according to Forbes. Time Magazine recognized John as a motivational speaker that helps people find a “Sense of Meaning” in their lives.

#### Tom Sauer, TechStars Mentor
An early-stage startup veteran, Tom has been growing revenue operations for VC backed companies for over 10 years. Web.com acquired the first startup he joined in 2016 and Groupon acquired the 2nd in the same year. As the first employee at Fundera, he built out the companies revenue operations to originate nearly a half billion dollars of transactions in the companies first three years. Tom is an active angel investor and TechStars mentor but helps startups and companies of all sizes all over the world.

#### Taylor Grant, Angel Investor
Taylor is an experienced investment professional and angel investor, specializing in consumer products and tech. He has a decade of experience in the asset management industry. Taylor has also been an active cryptocurrencyandtokeninvestor,focusingonlong-term capital appreciation. Taylor received his BS in Finance & Ethics from Bentley University and holds the Series 7 & 66 licenses.


### Conclusion

Our vision is an open-source token standard for transferring crypto real estate securities on the blockchain in a legally compliant manner. The Returns Token can only transfer when Governor Service approves it. The Governor Service has the permissions needed for all regulatory compliance and also relays on off-chain marketplace control room to keep the code updated in this rapidly changing legal and technical climate. Due to our programming with the right rules set, the Returns Token enables ERC-20 tokens to become compliant crypto real estate securities that can be traded across any ERC-20 compatible platform.


References

Stephen McKeon. Traditional Asset Tokenization. Accessed: 2018-01-30. Aug. 2017.
Hackernoon.com/traditional-asset-tokenization

Rule 506 (b) of Regulation D, 17 C.F.R. 230.506.
SEC Rule 506, 230.506

Pavel Krachenko. Assets Will Be Tokens (and It Will Change Finance) Nov. 2017.
Coindesk.com/tokenization-will-make-assets-more-valuable

Aswath Damodaran. Marketing and Value: Measuring the Illiquidity Discount.
People.stern.nyc.edu

Bert Teuben, Shrenik Shah, and Hariharan G.G. Real Estate Market Size 2016.
Savills.co/uk/research_articles

EtherScan.io Showing the Top 10,000 Accounts by Ether Value.
Etherscan.io/accounts

The Cryptocurrency Market Showing Over $250,000,000. CoinMarketCap.com


### Disclaimer

This white paper (“White Paper”) is meant to describe the currently anticipated plans of RealtyReturns Global, Ltd. (“RealtyReturns”) for developing a new blockchain token mechanism (“Returns Token”), which plans be an open-sourced industry standard that defines a mechanism in which asset-back tokens can be compliantly transferred on the blockchain (“Returns Token”). Nothing in this document should be treated or read as a guarantee or promise of how the Access Token or Returns Token will develop oroftheutilityorvalue ofthe Access Token and Returns Token.

This White Paper outlines RealtyReturns’s current plans, which could change at its discretion, and the success of which will depend on many factors outside RealtyReturns control, including market-based factors and factors within the data and cryptocurrency industries, among others. Any statements about future events are based solely on RealtyReturns analysis of the issues described in these documents. That analysis may prove to be incorrect. This document does not constitute an offer or sale of Access Token or Returns Token or any other mechanism for purchasing the Access Token and Returns Token (such as, without limitation, a “Simple Agreement for Future Tokens” related to Access Token and Returns Token. Any offer or sale of the Access Token and Returns Token or any related instrument will occur only based on final offering documents for Access Token and Returns Token for the applicable instrument.
CAUTIONARY NOTE ON FORWARD-LOOKING STATEMENTS

This Whitepaper may contain forward-looking statements including, but not limited to, statements as to future operating results and plans that involve risks and uncertainties. The use of words such as “expects”, “anticipates”, “believes”, “estimates”, the negative of these terms and similar expressions identify forward-looking statements. Such forward-looking statements involve known and unknown risks, uncertainties and other factors which may cause the actual results, performance or achievements of RealtyReturns to differ materially from any future results, performance or achievements expressed or implied by those projected in the forward-looking statements for any reason.
NO ADVICE

NoinformationinthisWhitepapershouldbeconsideredbusiness,legal,financialortaxadviceregarding RealtyReturns, the Tokens or any future Token sale or distribution. You should consult your own legal, financial, tax or other professional adviser regarding RealtyReturns, and its business and operations and the Tokens. You may be required to bear the financial risk of any purchase of the Tokens for an indefinite period of time or suffer the complete loss of any amounts paid for the Tokens.
RESTRICTIONS ON DISTRIBUTION AND DISSEMINATION

The distribution or dissemination of this Whitepaper or any part thereof may be prohibited or restricted by the laws, regulatory requirements and rules of any jurisdiction. In the case where any restriction applies, you are to inform yourself about, and to observe, any restrictions which are applicable to your possession of this Whitepaper or such part thereof (as the case may be) at your own expense and without liability to RealtyReturns or its affiliates. Persons to whom a copy of this Whitepaper has been distributed or disseminated or who have been provided access or otherwise have the Whitepaper in their possession shall not circulate it to any other persons, reproduce or otherwise distribute this Whitepaper or any information contained herein for any purpose whatsoever nor permit or cause the same to occur.
NO OFFER OF SECURITIES OR REGISTRATION

This Whitepaper does not constitute a prospectus or offer document of any sort and is not intended to constitute an offer of securities or a solicitation for investments in securities in any jurisdiction. No person is bound to enter into any contract or binding legal commitment, and no cryptocurrency or other form ofpaymentistobeacceptedbasedonthis Whitepaper. Anyagreementrelatingtothesale and purchase of the Tokens is to be governed solely by the Purchase Documents as RealtyReturns may require and no other document (including this Whitepaper).
RealtyReturns White Paper 22	


### RISKS AND UNCERTAINTIES

Prospective purchasers of Tokens should carefully consider and evaluate all risks and uncertainties associated with RealtyReturns and its plans, business and operations, the Tokens and any sale or distribution thereof, including all information set out in this Whitepaper and the Purchase Document prior to any purchase of the Tokens. If any of such risks and uncertainties develop into actual events, the business, financial condition, results of operations and prospects of RealtyReturns could be materially and adversely affected. In such cases, you may lose all or part of the value of any investment in the Tokens.
NOTICES FOR PARTICULAR INVESTORS

For residents of the People’s Republic of China (which, for the purposes of this Whitepaper, does not include Hong Kong, Macau, and Taiwan) only: The Tokens may not be marketed, offered or solddirectly orindirectly to the public inthe People’s Republic of China (the “PRC”) and neitherthis Whitepaper nor the Purchase Documents, which has not been submitted to the PRC securities and regulatory commission, nor any offering material or information contained herein relating to the Tokens, may be supplied to the public in the PRC or used in connection with any offer for the subscription or sale of the Tokens to the public in the PRC. The information contained in this Whitepaper and the Purchase Documents will not constitute an offer to sell or an invitation, advertisement or solicitation of an offer to buy any Tokens within the PRC.

Residents of the United States or any country subject to sanctions from the United States, including without limitation Belarus, Burundi, Central African Republic, Cuba, Iran, Libya, North Korea, Somalia, Sudan and Darfur, Syria and Zimbabwe, will not be permitted to purchase Tokens.


### Appendix

1: Smart Contract:
A Smart Contract is a protocol used to digitally facilitate, enforce and validate an online transaction. A smart contract allows two parties to securely perform online transactions without the need for third party validation.

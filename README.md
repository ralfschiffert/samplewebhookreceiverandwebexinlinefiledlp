# samplewebhookreceiverandwebexinlinefiledlp
sets up a webhook receiver and simulates a CASB in a terminal - runs as shell scripts


this is related to developer.webex.com to show inline file DLP functionality in simple scripts
the setupWebhokReceiver sets up a webhookinbox which is a 3rd party service to receive webhooks, this way this is serverless
call it as setupWebhokReceiver ${COTOKEN} with COTOKEN being the compliance officer token from developer.webex.com

the simulateCASB is also called with simulateCASB ${COTOKEN}
it polls from the webhookinbox and then asks interactively if to approve or reject the file

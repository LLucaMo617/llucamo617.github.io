# llucamo617.github.io
Site to host the geo caster site

<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GeoCaster Documentation</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }
        h1, h2, h3 {
            border-bottom: 2px solid #eee;
            padding-bottom: 5px;
            margin-top: 30px;
        }
        /* Stile opzionale per evidenziare gli ID (gli anchor) se vuoi vederli nel browser, altrimenti non necessario */
        /* [id]:before { content: "#" attr(id); display: block; margin-top: -50px; padding-top: 50px; color: #aaa; font-size: 0.8em; } */
    </style>
</head>
<body>

    <h1 id="documentazione_geocaster">GeoCaster Documentation</h1>

    <h2 id="overview">Overview</h2>
    <p id="overview_paragrafo_1">GeoCaster is a monday.com app that allows you to instantly transform a text address into a precise location on a map, which you can then visualize on a Map View within monday.com, all in one click.</p>

    <h3 id="what_is_geocoding">What is Geocoding?</h3>
    <p id="geocoding_paragrafo_1">Geocoding is the process of translating a text address—such as a postal code, city name, or street address—into geographic coordinates. In monday.com, this allows you to plot vital information—like customer locations, event venues, or property listings—on a geographical map for better visualization and planning.</p>

    <h3 id="important_note">Important Note</h3>
    <p id="important_note_paragrafo_1">The current version of the app only supports geocoding (casting a text address into a location column); it does not support the opposite process (reverse geocoding).</p>

    <h2 id="key_features">Key Features & Use Cases</h2>

    <p id="key_features_paragrafo_1">GeoCaster can be leveraged across various industries for enhanced geographic data visualization and planning:</p>
    <ul>
        <li id="use_case_sales"><strong>Sales & CRM:</strong> Map a new lead's location before a meeting or visualize your entire client base to better understand and optimize your sales territories.</li>
        <li id="use_case_real_estate"><strong>Real Estate:</strong> Geocode property listings quickly to create a visual portfolio of available sites for your clients.</li>
        <li id="use_case_logistics"><strong>Logistics & Field Services:</strong> Convert service addresses or delivery points into mappable locations for easier planning and efficient route optimization.</li>
        <li id="use_case_event_planners"><strong>Event Planners:</strong> Plot vendor locations, event venues, and attendee addresses to coordinate your efforts with geographic precision.</li>
    </ul>

    <h2 id="getting_started">Getting Started</h2>

    <h3 id="installation">Installation</h3>
    <p id="installation_paragrafo_1">You can add GeoCaster directly from the monday.com marketplace or by clicking [here]. Doing so will direct you to your monday.com account to complete the installation.</p>

    <h3 id="seamless_setup">Seamless Setup (Integration Guide)</h3>
    <p id="seamless_setup_paragrafo_1">GeoCaster runs on a simple, set-it-and-forget-it integration recipe. The process activates the moment you enter an address and click the button on your column.</p>
    <p id="seamless_setup_paragrafo_2">To set up the integration, we recommend having both a Text column and a Location column ready on your monday.com board.</p>

    <h4 id="steps_to_set_up">Steps to Set Up the Integration</h4>
    <ol>
        <li id="step_1_navigate">Navigate to “Integrate” within the monday.com board that contains the data you wish to translate into locations.</li>
        <li id="step_2_search">Search for GeoCaster among the available integrations and apps.</li>
        <li id="step_3_click_box">Click on the GeoCaster box to be redirected to the app's integration recipes page.</li>
        <li id="step_4_add_recipe">Click on “Add recipe” to proceed to the set-up page.</li>
        <li id="step_5_select_columns">Select the mandatory columns to fill in the placeholders:
            <ul>
                <li>**Button:** Select a button column on your board.</li>
                <li>**Address:** Build your address using the information contained in one or more text-type columns within your board.</li>
                <li>**Location:** Select a location-type column on your board.</li>
            </ul>
        </li>
        <li id="step_6_add_column_note">(If you don’t already have a text and a location column, you can click on “add column” to create them.)</li>
        <li id="step_7_finalize">Click on “Add Automation” to finalize the setup.</li>
    </ol>

    <h2 id="technical_legal">Technical & Legal Details</h2>

    <h3 id="external_services">External Services</h3>
    <p id="external_services_paragrafo_1">The GeoCaster app backend is based on Make.com.</p>
    <p id="external_services_paragrafo_2">The app uses the Google Maps Geocoding API to retrieve the coordinates for your addresses. You can find a detailed deep-dive of Google Maps Geocoding data treatment at a dedicated documentation link.</p>

    <h3 id="privacy_security">Privacy & Security</h3>
    <p id="privacy_security_paragrafo_1">All data is encrypted in transit and at rest in our backend. For a comprehensive overview, please refer to our Privacy & Security policy, available [here].</p>

    <h3 id="monday_account_info">monday.com Account Information</h3>
    <p id="monday_account_info_paragrafo_1">We store your account information (admin name, admin email address, account name, and slug) for providing you with necessary support. We do not have access to your credit card details at any time. We recommend you refer to the [payment service] Terms and Conditions for information about payment data handling.</p>

    <h3 id="monday_account_content">monday.com Account Content</h3>
    <p id="monday_account_content_paragrafo_1">We read board content (specifically, only the item that triggers the geocoding action), but we do not store any information contained in the communication between monday.com, the app, and Google Maps. We recommend you also refer to our Privacy & Security policy, available [here].</p>

    <h3 id="terms_of_service">Terms of Service</h3>
    <p id="terms_of_service_paragrafo_1">For a comprehensive overview of our service agreements, please refer to our Terms & Conditions, which is available [here].</p>

    <h2 id="privacy_security_policy_detail">Privacy & Security Policy</h2>
    <p id="privacy_policy_detail_paragrafo_1">il backend dell’app è interamente contenuto nei server make.com e pertanto vengono applicate le policy di privacy & security della piattaforma make.com stessa.</p>
    <p id="privacy_policy_detail_paragrafo_2">l’unico secret utilizzato è il token JWT generato da monday ed utilizzato, nei limiti temporali definiti da monday stessa, per le comunicazioni con monday, nello specifico nel recupero delle informazioni dell’account che ha inizializzato l’operazione, recupero dei dati presenti nell’item che ha triggerato l’applicazione e la compilazione della colonna di destinazione dell’output. I dati recuperati dall’item trigger vengono inviati a google Maps per la geolocalizzazione. Tutti questi dati non vengono salvati e rimangono nei server per il tempo strettamente necessario alla loro elaborazione. Tutte le comunicazioni in entrata ed in uscita sono criptate secondo TLS version 1.2 and 1.3 using AES 256 encryption (refer to make.com documentation).</p>

    <hr>
    
    <h2 id="install_button">Bottone Installazione</h2>
    <p>Clicca sul bottone per aggiungere GeoCaster al tuo account monday.com.</p>
    
    <a href="https://auth.monday.com/oauth2/authorize?client_id=4f8bcf23e5516e2994ea27a3188fad66&response_type=install">
      <img
        alt="Add to monday.com"
        height="32"
        src="https://dapulse-res.cloudinary.com/image/upload/f_auto,q_auto/remote_mondaycom_static/uploads/Tal/4b5d9548-0598-436e-a5b6-9bc5f29ee1d9_Group12441.png"
      />
    </a>

</body>
</html>

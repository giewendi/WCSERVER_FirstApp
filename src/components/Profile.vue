<template>
    <div id="profile">
        <h2>{{title}}</h2>
        <div id="info">
            <table>
                <thead>
                    <tr>
                        <th colspan="2">Personal Information</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Date of Birth</td>
                        <td>{{birth}}</td>
                    </tr>
                    <tr>
                        <td>Nationality</td>
                        <td>{{nationality}}</td>
                    </tr>
                    <tr>
                        <td>Marital Status</td>
                        <td>{{marital}}</td>
                    </tr>
                    <tr>
                        <td>Language</td>
                        <td>{{lang1}} <br>{{lang2}} <br>{{lang3}}</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>
</template>

<script>
export default {
    name: 'profile',
    data () {
        return {
            title: 'Profile',
            birth: "02/22/2002",
            nationality: "Filipino",
            marital: "Single",
            lang1: "Tagalog",
            lang2: "English",
            lang3: "Kapampangan"
        }
    }
}
</script>

<style>
#info{
    text-align: center;
}

#info table{
    filter: drop-shadow(0 0 1px rgb(61, 49, 34));
    margin: 1em auto 0;
    margin-right: auto;
    font-size: large;
}

#info td, #info th{
    background: white;
    filter: drop-shadow(0 0 1px rgb(61, 49, 34));
    padding: 1em 10em;
}

#info th{
    font-size:larger;
}

#info tr{
    margin: 1em;
}
</style>
# bpjs-check

The BPJS Check is an online service designed to help individuals verify their membership status in the BPJS Kesehatan program, which is Indonesia's national health insurance scheme. This service allows users to easily access information regarding their health insurance coverage, ensuring that they are aware of their rights and benefits under the program.

Key Features:
Membership Verification: Users can input their National Identification Number (NIK) or No Kartu Bpjs to check if they are registered as BPJS Kesehatan participants.

Real-Time Information: The service provides real-time updates on the status of the user's membership, including active status, coverage details, and any potential issues that may need to be addressed.

User -Friendly Interface: The BPJS Check service is designed to be intuitive and easy to navigate, making it accessible for all users, regardless of their technical expertise.

Secure Access: The platform ensures that user data is handled securely, maintaining privacy and confidentiality throughout the verification process.

Support for Participants: In addition to checking membership status, the service may offer guidance on how to resolve issues related to registration, claims, and benefits.

Importance:
The BPJS Check service is crucial for ensuring that individuals are aware of their health insurance status, which is essential for accessing medical services and benefits. By providing a straightforward way to verify membership, the service helps promote awareness and utilization of the BPJS Kesehatan program, ultimately contributing to better health outcomes for the population.

In summary, the BPJS Check is a vital tool for Indonesian citizens to manage their health insurance effectively, ensuring they receive the necessary care and support when needed.

```
const options = {
  method: 'POST',
  headers: {
    'X-RapidAPI-Key': 'key',
    'X-RapidAPI-Host': 'check-bpjs.p.rapidapi.com'
  },
  body: 'noka=10863123'
};

fetch('https://check-bpjs.p.rapidapi.com/jkn', options)
  .then(response =&gt; response.json())
  .then(response =&gt; console.log(response))
  .catch(err =&gt; console.error(err));
```


RESULT

```
{
  "status": true,
  "data": {
    "nokartu": "0000010863167",
    "nik": "12082331109234",
    "nama": "NAMA",
    "jenis_kelamin": "Laki-Laki",
    "pisa": "1",
    "tgl_lahir": "1995-10-31",
    "tgl_cetak_kartu": "2025-01-01",
    "tgl_tat": "2050-12-31",
    "tgl_tmt": "1996-09-12",
    "status": "0 - AKTIF",
    "kelurahan": "02071701 - BOSAR MALIGAS",
    "hak_kelas": "1 - KELAS I",
    "jenis_peserta": "13 - PEGAWAI SWASTA",
    "umur_skrg": "29 tahun, 3 bulan, 22 hari - 29 tahun, 3 bulan, 22 hari",
    "noMR": null,
    "noTelepon": null
  }
}
```

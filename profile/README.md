```python
class Agency:
    def __init__(self, name, services, description, contact_info):
        self.name = name
        self.services = services
        self.description = description
        self.contact_info = contact_info

    def describe_agency(self):
        description = f"🌟 Welcome to {self.name} 🌟\n"
        description += "=" * len(description) + "\n\n"
        description += f"{self.description}\n\n"
        description += "🔧 **Our Services:**\n"
        for service in self.services:
            description += f"    - {service}\n"
        description += "\n📞 **Contact Us:**\n"
        description += f"    - Email: {self.contact_info['email']}\n"
        description += f"    - Phone: {self.contact_info['phone']}\n"
        description += "\n" + "=" * len(description) + "\n"
        description += "Thank you for considering our services!\n"
        return description

agency_name = "Tuxedo Labs"
agency_services = [
    "Jasa pembuatan website",
    "Konsultasi dan perencanaan proyek",
    "Desain UI/UX",
    "Pengembangan aplikasi web",
    "Pemeliharaan dan dukungan teknis"
]
agency_description = (
    "At Tuxedo Labs, we are committed to delivering top-notch web solutions "
    "that are tailored to meet your business needs. Our expert team combines "
    "creativity and technical skills to craft stunning, user-friendly websites "
    "that not only look great but also perform seamlessly."
)

agency_contact_info = {
    "email": "rafia9005@gmail.com",
    "phone": "+6282143338737",
}

tuxedo_labs = Agency(
    name=agency_name,
    services=agency_services,
    description=agency_description,
    contact_info=agency_contact_info
)

print(tuxedo_labs.describe_agency())
```

# <a name="microsoft-bookings-api-overview-preview"></a>Обзор API Microsoft Bookings (предварительная версия)

В случае Microsoft Bookings доступны мобильные и интернет-приложения, обеспечивающие простое и эффективное планирование встреч для небольших компаний и их клиентов. Небольшие компании, которые предоставляют услуги, предусматривающие планирование встреч (например, автомастерские, парикмахерские, юридические фирмы), смогут освободить время, отведенное на управление резервированием, и потратить его на более важные задачи для развития бизнеса. Служба Microsoft Bookings доступна для компаний с подпиской на Office 365 бизнес премиум.

## <a name="why-integrate-with-microsoft-bookings-using-microsoft-graph"></a>Зачем проводить интеграцию с Microsoft Bookings, используя Microsoft Graph?

### <a name="streamline-appointment-booking"></a>Простое планирование встреч
Предприниматель никогда не пропустит случаи резервации, когда находится вдали от телефона или когда фирма закрывается. Клиенты могут [видеть доступные услуги](../api-reference/beta/api/bookingbusiness_list_services.md) и [резервировать их на определенное время](../api-reference/beta/api/bookingbusiness_post_appointments.md) в любой момент прямо на странице планирования, на Facebook или веб-сайте компании. 

Предприниматели могут подтверждать резервацию в мобильном или интернет-приложении, лично или по телефону. Они могут [перенести](../api-reference/beta//api/bookingappointment_update.md) или [отменить](../api-reference/beta/api/bookingappointment_cancel.md) бронь, а также [переназначить](../api-reference/beta/api/bookingappointment_update.md) ее, указав другого доступного сотрудника. 

### <a name="reduce-no-shows-and-increase-productivity-of-the-staff"></a>Сокращение количества неявок и увеличение эффективности сотрудников
Предприниматели могут указать [политики планирования](../api-reference/beta/resources/bookingschedulingpolicy.md), включающие минимальные уведомления о резервировании и отмене, а клиенты могут планировать и переносить встречи самостоятельно. Автоматические подтверждения встреч и напоминания позволяют сократить количество неявок и эффективнее использовать рабочее время. 

### <a name="manage-customer-information-and-relationships-from-anywhere"></a>Управление сведениями о клиентах и соответствующих отношениях с любого устройства
При добавлении встречи автоматически проверяется, указан ли человек в [списке клиентов](../api-reference/beta/api/bookingbusiness_list_customers.md), и при необходимости [добавляются](../api-reference/beta/api/bookingbusiness_post_customers.md) его имя и электронный адрес в этот список. Благодаря этому предприниматели могут с легкостью оставаться на связи с клиентами и периодически отправлять им информационные бюллетени и другие рекламные материалы.

### <a name="integrate-with-productivity-and-team-collaboration-services-in-microsoft-graph"></a>Интеграция со службами, повышающими эффективность работы и сотрудничества, в Microsoft Graph
Используя единую конечную точку REST Microsoft Graph, вы можете получить доступ к API Bookings и [интегрировать лучшее из Microsoft 365](overview-major-services.md) для поддержки многофункциональных сценариев. Например, с помощью [Excel](excel-concept-overview.md#generate-reports-and-analyze-results) вы можете отслеживать и анализировать финансовые данные компании, создавать профессиональные отчеты, а с помощью [SharePoint](sharepoint-concept-overview.md) или [Microsoft Teams](teams-concept-overview.md) — повысить эффективность сотрудничества команд.

## <a name="next-steps"></a>Дальнейшие действия

Дополнительные сведения:

- [Microsoft Bookings](https://support.office.com/en-us/article/Publish-your-business-calendar-online-with-Microsoft-Bookings-47403d64-a067-4754-9ae9-00157244c27d) и другие [приложения Office 365 бизнес](https://support.office.com/en-us/article/manage-your-business-apps-in-the-business-center-47eca808-cf96-42ba-83e8-55daf18e49dc?ui=en-US&rs=en-US&ad=US).
- [Использование API Bookings](../api-reference/beta/resources/booking-api-overview.md) в Microsoft Graph.


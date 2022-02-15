---
title: тип ресурса organizationalBrandingProperties
description: Содержит сведения о брендинге организации.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 68831b6069df0ea94df36605ff9f1099dfd27feb
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2022
ms.locfileid: "62805146"
---
# <a name="organizationalbrandingproperties-resource-type"></a>тип ресурса organizationalBrandingProperties

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактный тип, который предоставляет свойства для настройки фирменого бренда организации.

Организации могут настраивать Azure Active Directory (Azure AD), которые отображаются при входе пользователей в конкретные приложения организации или когда Azure AD идентифицирует клиента пользователя из имени пользователя. Разработчик также может ознакомиться с информацией о брендинге компании и настроить интерфейс приложения, чтобы настроить его специально для пользователя, вписаного в нее, с помощью фирменого бренда.

Вы не можете изменить язык исходной конфигурации, представленный [объектом organizationalBranding](organizationalbranding.md) . Тем не менее, компании могут добавлять различные брендинги на основе локального. Для языкового брендинга см. объект [organizationalBrandingLocalization](organizationalbrandinglocalization.md) .

>[!NOTE]
>Добавление настраиваемой фирменой марки требует лицензий Azure Active Directory (Azure AD) Premium 1, Premium 2 или Office 365 (для Office 365 приложений). Дополнительные сведения о лицензировании и выпусках см. в [Azure AD Premium.](/azure/active-directory/fundamentals/active-directory-get-started-premium)
>
>Azure AD Premium доступны для клиентов в Китае с помощью всемирного экземпляра Azure Active Directory. Azure AD Premium в настоящее время не поддерживается в службе Azure, выполняемой 21Vianet в Китае. Дополнительные сведения можно получить с помощью [Azure Active Directory Forum](https://feedback.azure.com/forums/169401-azure-active-directory/).

## <a name="methods"></a>Методы
Нет.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| backgroundColor | String | Цвет, который отображается на месте фонового изображения в подключениях с низкой пропускной способностью. Рекомендуется использовать основной цвет логотипа баннера или цвета организации. Укажите это в hexadecimal формате, например, белый .`#FFFFFF` |
| backgroundImage | Stream | Изображение, которое отображается в качестве фона страницы регистрации. Допустимые типы PNG или JPEG не меньше 300 КБ и не более 1920 × 1080 пикселей. Меньшее изображение уменьшит требования к пропускной способности и сделает загрузку страницы быстрее. |
| backgroundImageRelativeUrl | String | Относительный URL-адрес для свойства **backgroundImage**, который сочетается с базовым URL CDN из **cdnList**, чтобы предоставить версию, обслуживаемую CDN. Только для чтения. |
| bannerLogo | Stream | Баннерная версия логотипа вашей компании, которая отображается на странице входного знака. Допустимые типы PNG или JPEG не более 36 × 245 пикселей. Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа. |
| bannerLogoRelativeUrl | String | Относительный URL-адрес свойства **bannerLogo**, который сочетается с базовым URL-адресом CDN из **cdnList**, чтобы предоставить только для чтения версию, обслуживаемую CDN. Только для чтения. |
| cdnList | Коллекция String | Список базовых URL-адресов для всех CDN поставщиков, обслуживающих активы текущего ресурса. Несколько CDN одновременно используются для обеспечения высокой доступности запросов на чтение. Только для чтения. |
| customAccountResetCredentialsUrl | String | Настраиваемый URL-адрес для сброса учетных данных учетных записей. Этот URL-адрес должен быть в формате ASCII или символы, не вносимые в ASCII, должны быть закодированы и не превышать 128 символов. |
| customCannotAccessYourAccountText | String | Строка для замены по умолчанию "Не может получить доступ к учетной записи?" текст гиперссылки самообслуживляемого сброса пароля (SSPR) на странице вход. Этот текст должен быть в формате Unicode и не превышать 256 символов. |
| customCannotAccessYourAccountUrl | String | Пользовательский URL-адрес для замены URL-адреса сброшенного пароля самообслуживной службы (SSPR) "Не может получить доступ к вашей учетной записи?" гиперссылка на странице вход. Этот URL-адрес должен быть в формате ASCII или символы, не вносимые в ASCII, должны быть закодированы и не превышать 128 символов. <br/><br/>**НЕ ИСПОЛЬЗУЙТЕ.** Вместо **этого используйте customAccountResetCredentialsUrl** . |
| customForgotMyPasswordText | String | Строка для замены текста гиперссылки по умолчанию "Забыл пароль" в форме входного знака. Этот текст должен быть в формате Unicode и не превышать 256 символов. |
| customPrivacyAndCookiesText | String | Строка для замены текста гиперссылки "Конфиденциальность и файлы cookie" в подножке. Этот текст должен быть в формате Unicode и не превышать 256 символов. |
| customPrivacyAndCookiesUrl | String | Пользовательский URL-адрес для замены URL-адреса гиперссылки "Конфиденциальность и файлы cookie" в подножке. Этот URL-адрес должен быть в формате ASCII или символы, не вносимые в ASCII, должны быть закодированы и не превышать 128 символов. |
| customResetItNowText | String | Строка для замены текста гиперссылки по умолчанию "сбросим его сейчас" в форме входного знака. Этот текст должен быть в формате Unicode и не превышать 256 символов. <br/><br/>**НЕ ИСПОЛЬЗУЙТЕ:** Настройка текста гиперссылки "сброс сейчас" в настоящее время не поддерживается. |
| customTermsOfUseText | String | Строка для замены текста гиперссылки по умолчанию "Термины использования" в подножке. Этот текст должен быть в формате Unicode и не превышать 256 символов. |
| customTermsOfUseUrl | String | Пользовательский URL-адрес для замены URL-адреса гиперссылки "Условия использования" в подножке. Этот URL-адрес должен быть в формате ASCII или символы, не вносимые в ASCII, должны быть закодированы и не превышать 128characters. |
| favicon | Stream | Настраиваемый значок (favicon) для замены фавикона продукта Microsoft по умолчанию на клиенте Azure AD. |
| faviconRelativeUrl | String | Относительный URL-адрес для викона выше, который CDN базовый URL-адрес **из cdnList**, чтобы предоставить версию, обслуживаемую CDN. Только для чтения. |
| headerBackgroundColor | String | Цвет RGB, который необходимо применить для настройки цвета загона. |
| id | String | Идентификатор, который представляет указанный локальный код с использованием имен культуры. Имена культур следуют стандарту RFC 1766 в формате "languagecode2-country/regioncode2", где "languagecode2" — это код из двух букв более низкого уровня, полученный из ISO 639-1, а "country/regioncode2" — это код с двумя буквами верхнего уровня, полученный из ISO 3166. Например, американский английский язык `en-US`. **Id** для по умолчанию /branding всегда типы строки `0` или .`default` Только для чтения. <br/><br/>**ПРИМЕЧАНИЕ:** Несколько фирменных окей для одного локального уровня в настоящее время не поддерживаются. |
| loginPageTextVisibilitySettings | [loginPageTextVisibilitySettings](loginPageTextVisibilitySettings.md) | Представляет различные тексты, которые можно скрыть на странице входа для клиента. |
| signInPageText | String | Текст, который отображается в нижней части окна для регистрации. Используйте это для получения дополнительных сведений, например номера телефона в службе поддержки или юридического заявления. Этот текст должен быть в формате Unicode и не превышать 1024 символов. |
| squareLogo | Stream | Квадратная версия логотипа вашей компании, которая отображается Windows 10 вне окна (OOBE) и когда Windows автопилот включен для развертывания. Допустимые типы PNG или JPEG не более 240 x 240 пикселей и не более 10 КБ в размере. Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.|
| squareLogoRelativeUrl | String | Относительный URL-адрес для свойства **squareLogo**, который CDN с базовым URL-адресом **из cdnList**, чтобы предоставить версию, обслуживаемую CDN. Только для чтения. |
| usernameHintText | String | Строка, отображаемая в виде подсказки в текстовом ящике имени пользователя на экране регистрации. Этот текст должен быть юникодом без ссылок или кода и не может превышать 64 символов. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organizationalBrandingProperties",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organizationalBrandingProperties",
  "id": "String (identifier)",
  "backgroundColor": "String",
  "backgroundImage": "Stream",
  "backgroundImageRelativeUrl": "String",
  "bannerLogo": "Stream",
  "bannerLogoRelativeUrl": "String",
  "cdnList": [
    "String"
  ],
  "signInPageText": "String",
  "squareLogo": "Stream",
  "squareLogoRelativeUrl": "String",
  "usernameHintText": "String",
  "customAccountResetCredentialsUrl": "String",
  "customCannotAccessYourAccountText": "String",
  "customCannotAccessYourAccountUrl": "String",
  "customForgotMyPasswordText": "String",
  "customPrivacyAndCookiesText": "String",
  "customPrivacyAndCookiesUrl": "String",
  "customResetItNowText": "String",
  "customTermsOfUseText": "String",
  "customTermsOfUseUrl": "String",
  "favicon": "Stream",
  "faviconRelativeUrl": "String",
  "headerBackgroundColor": "String",
  "loginPageTextVisibilitySettings": {
    "@odata.type": "microsoft.graph.loginPageTextVisibilitySettings"
  }
}
```

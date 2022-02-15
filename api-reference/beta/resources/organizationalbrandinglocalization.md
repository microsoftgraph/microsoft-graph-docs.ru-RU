---
title: тип ресурса organizationalBrandingLocalization
description: Содержит сведения о локализации брендинга организации.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b01a52bd81c5b1cbbaf8611ab0efd96c75f229b5
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804628"
---
# <a name="organizationalbrandinglocalization-resource-type"></a>тип ресурса organizationalBrandingLocalization

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс, поддерживаюющий управление языковым брендингом. Хотя вы не можете изменить язык исходной конфигурации, этот ресурс позволяет создать новую конфигурацию для другого языка.

Наследует от [organizationalBrandingProperties](organizationalbrandingproperties.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Списки организационныхбрандингЛокализации](../api/organizationalbranding-list-localizations.md)|Коллекция [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|Получите список объектов [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) и их свойств.|
|[Создание organizationalBrandingLocalization](../api/organizationalbranding-post-localizations.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|Создайте новый [объект organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) .|
|[Получение organizationalBrandingLocalization](../api/organizationalbrandinglocalization-get.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|Ознакомьтесь с свойствами и отношениями объекта [организационнойbrandingLocalization](../resources/organizationalbrandinglocalization.md) .|
|[Обновление organizationalBrandingLocalization](../api/organizationalbrandinglocalization-update.md)| Нет |Обновление свойств объекта [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) .|
|[Удаление organizationalBrandingLocalization](../api/organizationalbrandinglocalization-delete.md)|Нет|Удаляет объект [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) .|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| backgroundColor | String | Цвет, который отображается на месте фонового изображения в подключениях с низкой пропускной способностью. Рекомендуется использовать основной цвет логотипа баннера или цвета организации. Укажите это в hexadecimal формате, например, белый .`#FFFFFF` Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |
| backgroundImage | Stream | Изображение, которое отображается в качестве фона страницы регистрации. Допустимые типы PNG или JPEG не меньше 300 КБ и не более 1920 × 1080 пикселей. Меньшее изображение уменьшит требования к пропускной способности и сделает загрузку страницы быстрее. Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |
| backgroundImageRelativeUrl | String | Относительный URL-адрес для свойства **backgroundImage**, который сочетается с базовым URL CDN из **cdnList**, чтобы предоставить версию, обслуживаемую CDN. Только для чтения. Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |
| bannerLogo | Stream | Баннерная версия логотипа вашей компании, которая отображается на странице входного знака. Допустимые типы PNG или JPEG не более 36 × 245 пикселей. Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа. Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |
| bannerLogoRelativeUrl | String | Относительный URL-адрес свойства **bannerLogo**, который сочетается с базовым URL-адресом CDN из **cdnList**, чтобы предоставить только для чтения версию, обслуживаемую CDN. Только для чтения. Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |
| cdnList | Коллекция строк | Список базовых URL-адресов для всех CDN поставщиков, обслуживающих активы текущего ресурса. Несколько CDN одновременно используются для обеспечения высокой доступности запросов на чтение. Только для чтения. Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |
| customAccountResetCredentialsUrl | String | Настраиваемый URL-адрес для сброса учетных данных учетных записей. Этот URL-адрес должен быть в формате ASCII или символы, не вносимые в ASCII, должны быть закодированы и не превышать 128 символов. Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |
| customCannotAccessYourAccountText | String | Строка для замены по умолчанию "Не может получить доступ к учетной записи?" текст гиперссылки самообслуживляемого сброса пароля (SSPR) на странице вход. Этот текст должен быть в формате Unicode и не превышать 256 символов. Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |
| customCannotAccessYourAccountUrl | String | Пользовательский URL-адрес для замены URL-адреса сброшенного пароля самообслуживной службы (SSPR) "Не может получить доступ к вашей учетной записи?" гиперссылка на странице вход. Этот URL-адрес должен быть в формате ASCII или символы, не вносимые в ASCII, должны быть закодированы и не превышать 128 символов. <br/><br/>**НЕ ИСПОЛЬЗУЙТЕ.** Вместо **этого используйте customAccountResetCredentialsUrl** . Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |
| customForgotMyPasswordText | String | Строка для замены текста гиперссылки по умолчанию "Забыл пароль" в форме входного знака. Этот текст должен быть в формате Unicode и не превышать 256 символов. Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |
| customPrivacyAndCookiesText | String | Строка для замены текста гиперссылки "Конфиденциальность и файлы cookie" в подножке. Этот текст должен быть в формате Unicode и не превышать 256 символов. Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |
| customPrivacyAndCookiesUrl | String | Пользовательский URL-адрес для замены URL-адреса гиперссылки "Конфиденциальность и файлы cookie" в подножке. Этот URL-адрес должен быть в формате ASCII или символы, не вносимые в ASCII, должны быть закодированы и не превышать 128 символов. Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |
| customResetItNowText | String | Строка для замены текста гиперссылки по умолчанию "сбросим его сейчас" в форме входного знака. Этот текст должен быть в формате Unicode и не превышать 256 символов. <br/><br/>**НЕ ИСПОЛЬЗУЙТЕ:** Настройка текста гиперссылки "сброс сейчас" в настоящее время не поддерживается. Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |
| customTermsOfUseText | String | Строка для замены текста гиперссылки по умолчанию "Термины использования" в подножке. Этот текст должен быть в формате Unicode и не превышать 256 символов. Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |
| customTermsOfUseUrl | String | Пользовательский URL-адрес для замены URL-адреса гиперссылки "Условия использования" в подножке. Этот URL-адрес должен быть в формате ASCII или символы, не вносимые в ASCII, должны быть закодированы и не превышать 128characters. Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |
| favicon | Stream | Настраиваемый значок (favicon) для замены фавикона продукта Microsoft по умолчанию на клиенте Azure AD. Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |
| faviconRelativeUrl | String | Относительный URL-адрес для викона выше, который CDN базовый URL-адрес **из cdnList**, чтобы предоставить версию, обслуживаемую CDN. Только для чтения. Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |
| headerBackgroundColor | String | Цвет RGB, который необходимо применить для настройки цвета загона. Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |
| id | String | Идентификатор, который представляет указанный локальный код с использованием имен культуры. Имена культур следуют стандарту RFC 1766 в формате "languagecode2-country/regioncode2", где "languagecode2" — это код из двух букв более низкого уровня, полученный из ISO 639-1, а "country/regioncode2" — это код с двумя буквами верхнего уровня, полученный из ISO 3166. Например, американский английский язык `en-US`. **Id** для по умолчанию /branding всегда типы строки `0` или .`default` Только для чтения. <br/><br/>**ПРИМЕЧАНИЕ:** Несколько фирменных окей для одного локального уровня в настоящее время не поддерживаются. |
| loginPageTextVisibilitySettings | [loginPageTextVisibilitySettings](loginPageTextVisibilitySettings.md) | Представляет различные тексты, которые можно скрыть на странице входа для клиента. Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |
| signInPageText | String | Текст, который отображается в нижней части окна для регистрации. Используйте это для получения дополнительных сведений, например номера телефона в службе поддержки или юридического заявления. Этот текст должен быть в формате Unicode и не превышать 1024 символов. |
| squareLogo | Stream | Квадратная версия логотипа вашей компании, которая отображается Windows 10 вне окна (OOBE) и когда Windows автопилот включен для развертывания. Допустимые типы PNG или JPEG не более 240 x 240 пикселей и не более 10 КБ в размере. Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа. Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md).|
| squareLogoRelativeUrl | String | Относительный URL-адрес для свойства **squareLogo**, который CDN с базовым URL-адресом **из cdnList**, чтобы предоставить версию, обслуживаемую CDN. Только для чтения. Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |
| usernameHintText | String | Строка, отображаемая в виде подсказки в текстовом ящике имени пользователя на экране регистрации. Этот текст должен быть юникодом без ссылок или кода и не может превышать 64 символов. Наследуется [от organizationalBrandingProperties](organizationalbrandingproperties.md). |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organizationalBrandingLocalization",
  "baseType": "microsoft.graph.organizationalBrandingProperties",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organizationalBrandingLocalization",
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
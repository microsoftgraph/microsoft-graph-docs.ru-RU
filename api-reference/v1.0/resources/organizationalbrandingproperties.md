---
title: тип ресурса organizationalBrandingProperties
description: Содержит сведения о брендинге организации.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f97ff1378560094a400e5e2519903176334e768d
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647093"
---
# <a name="organizationalbrandingproperties-resource-type"></a>тип ресурса organizationalBrandingProperties

Пространство имен: microsoft.graph

Абстрактный тип, который предоставляет свойства для настройки фирменого бренда организации.

Организации могут настраивать Azure Active Directory (Azure AD), которые отображаются при входе пользователей в конкретные приложения организации или когда Azure AD идентифицирует клиента пользователя из имени пользователя. Разработчик также может ознакомиться с информацией о брендинге компании и настроить интерфейс приложения, чтобы настроить его специально для пользователя, вписаного в нее, с помощью фирменого бренда.

Вы не можете изменить язык исходной конфигурации, представленный [объектом organizationalBranding.](organizationalbranding.md) Тем не менее, компании могут добавлять различные брендинги на основе локального. Для языкового брендинга см. объект [organizationalBrandingLocalization.](organizationalbrandinglocalization.md)

>[!NOTE]
>Добавление настраиваемой фирменой марки требует лицензий Azure Active Directory (Azure AD) Premium 1, Premium 2 или Office 365 (для Office 365 приложений). Дополнительные сведения о лицензировании и выпусках см. в [Azure AD Premium.](/azure/active-directory/fundamentals/active-directory-get-started-premium)
>
>Azure AD Premium доступны для клиентов в Китае с помощью всемирного экземпляра Azure Active Directory. Azure AD Premium в настоящее время не поддерживается в службе Azure, выполняемой 21Vianet в Китае. Дополнительные сведения можно получить с помощью [Azure Active Directory Forum.](https://feedback.azure.com/forums/169401-azure-active-directory/)

## <a name="methods"></a>Методы
| Нет.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| backgroundColor | String | Цвет, который будет отображаться на месте фонового изображения в подключениях с низкой пропускной способностью. Рекомендуется использовать основной цвет логотипа баннера или цвета организации. Укажите это в hexadecimal формате, например, белый `#FFFFFF` . |
| backgroundImage | Stream | Изображение, которое отображается в качестве фона страницы регистрации. Допустимые типы PNG или JPEG не меньше 300 КБ и не более 1920 × 1080 пикселей. Меньшее изображение уменьшит требования к пропускной способности и сделает загрузку страницы быстрее. |
| backgroundImageRelativeUrl | String | Относительный URL-адрес свойства **backgroundImage,** который сочетается с базовым URL CDN из **cdnList,** чтобы предоставить версию, обслуживаемую CDN. Только для чтения. |
| bannerLogo | Stream | Баннерная версия логотипа вашей компании, которая отображается на странице входного знака. Допустимые типы PNG или JPEG не более 36 × 245 пикселей. Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа. |
| bannerLogoRelativeUrl | String | Относительный URL-адрес свойства **bannerLogo,** который сочетается с базовым URL-адресом CDN из **cdnList,** чтобы предоставить только для чтения версию, обслуживаемую CDN. Только для чтения. |
| cdnList | Коллекция String | Список базовых URL-адресов для всех CDN поставщиков, обслуживающих активы текущего ресурса. Несколько CDN одновременно используются для обеспечения высокой доступности запросов на чтение. Только для чтения. |
| id | String | Идентификатор, который представляет указанный локальный код с использованием имен культуры. Имена культур следуют стандарту RFC 1766 в формате "languagecode2-country/regioncode2", где "languagecode2" — это код из двух букв более низкого уровня, полученный из ISO 639-1, а "country/regioncode2" — это код с двумя буквами верхнего уровня, полученный из ISO 3166. Например, американский английский язык `en-US` . **Id** для по умолчанию /branding всегда типы `0` строки или `default` . Только для чтения. <br/><br/>**ПРИМЕЧАНИЕ:** Несколько фирменных окей для одного локального уровня в настоящее время не поддерживаются. |
| signInPageText | String | Текст, который отображается в нижней части окна для регистрации. С помощью этого можно сообщить дополнительные сведения, например номер телефона в службу поддержки или юридический отчет. Этот текст должен быть unicode и не превышать 1024 символов. |
| squareLogo | Stream | Квадратная версия логотипа вашей компании, которая отображается Windows 10 вне окна (OOBE) и когда Windows автопилот включен для развертывания. Разрешены типы PNG или JPEG размером не более 240 x 240 пикселей и размером не более 10 КБ. Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа. |
| squareLogoRelativeUrl | String | Относительный URL-адрес для свойства **squareLogo,** который CDN базовый URL-адрес **из cdnList** для предоставления версии, обслуживаемой CDN. Только для чтения. |
| usernameHintText | String | Строка, отображаемая в виде подсказки в текстовом ящике имени пользователя на экране входной записи. Этот текст должен быть юникодом без ссылок или кода и не может превышать 64 символов. |

## <a name="relationships"></a>Отношения
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
  "@odata.type": "#microsoft.graph.organizationalBranding",
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
  "usernameHintText": "String"
}
```


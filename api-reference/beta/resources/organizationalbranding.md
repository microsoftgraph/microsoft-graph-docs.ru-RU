---
title: тип ресурса organizationalBranding
description: Содержит сведения о брендинге организации.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 44472ad122ff1fd2f9e7b23db705e6d077ead173
ms.sourcegitcommit: 6cea9bc17d3859e475a74c4a6f661f848e837e89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/08/2021
ms.locfileid: "60240784"
---
# <a name="organizationalbranding-resource-type"></a>тип ресурса organizationalBranding

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о брендинге организации по умолчанию. Наследует от [organizationalBrandingProperties](organizationalbrandingproperties.md).

Организации могут настраивать Azure Active Directory (Azure AD), которые отображаются при входе пользователей в конкретные приложения организации или когда Azure AD идентифицирует клиента пользователя из имени пользователя. Разработчик также может ознакомиться с информацией о брендинге компании и настроить интерфейс приложения, чтобы настроить его специально для пользователя, вписаного в нее, с помощью фирменого бренда.

Вы не можете изменить язык исходной конфигурации. Тем не менее, компании могут добавлять различные брендинги на основе локального. Для языкового брендинга см. объект [organizationalBrandingLocalization.](organizationalbrandingproperties.md)

>[!NOTE]
>Добавление настраиваемой фирменой марки требует лицензий Azure Active Directory (Azure AD) Premium 1, Premium 2 или Office 365 (для Office 365 приложений). Дополнительные сведения о лицензировании и выпусках см. в [Azure AD Premium.](/azure/active-directory/fundamentals/active-directory-get-started-premium)
>
>Azure AD Premium доступны для клиентов в Китае с помощью всемирного экземпляра Azure Active Directory. Azure AD Premium в настоящее время не поддерживается в службе Azure, выполняемой 21Vianet в Китае. Дополнительные сведения можно получить с помощью [Azure Active Directory Forum.](https://feedback.azure.com/forums/169401-azure-active-directory/)

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Получение organizationalBranding](../api/organizationalbranding-get.md) | [organizationalBranding](../resources/organizationalbranding.md) | Ознакомьтесь с свойствами и отношениями объекта [organizationalBranding.](../resources/organizationalbranding.md) |
| [Обновление organizationalBranding](../api/organizationalbranding-update.md) | Нет | Обновление свойств объекта [organizationalBranding.](../resources/organizationalbranding.md) |
<!--| [Удаление organizationalBranding](../api/organizationalbranding-delete.md) | Нет | Удаление [объекта organizationalBranding.](../resources/organizationalbranding.md) |-->

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| backgroundColor | Строка | Цвет, который будет отображаться на месте фонового изображения в подключениях с низкой пропускной способностью. Рекомендуется использовать основной цвет логотипа баннера или цвета организации. Укажите это в hexadecimal формате, например, белый `#FFFFFF` . Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| backgroundImage | Stream | Изображение, которое отображается в качестве фона страницы регистрации. Допустимые типы PNG или JPEG не меньше 300 КБ и не более 1920 × 1080 пикселей. Меньшее изображение уменьшит требования к пропускной способности и сделает загрузку страницы быстрее. Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Возвращается только на `$select`. |
| backgroundImageRelativeUrl | String | Относительный URL-адрес свойства **backgroundImage,** который сочетается с базовым URL CDN из **cdnList,** чтобы предоставить версию, обслуживаемую CDN. Только для чтения. Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| bannerLogo | Stream | Баннерная версия логотипа вашей компании, которая отображается на странице входного знака. Допустимые типы PNG или JPEG не более 36 × 245 пикселей. Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа. Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Возвращается только с помощью оператора `$select`. |
| bannerLogoRelativeUrl | Строка | Относительный URL-адрес свойства **bannerLogo,** который сочетается с базовым URL-адресом CDN из **cdnList,** чтобы предоставить только для чтения версию, обслуживаемую CDN. Только для чтения. Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| cdnList | Коллекция строк | Список базовых URL-адресов для всех CDN поставщиков, обслуживающих активы текущего ресурса. Несколько CDN одновременно используются для обеспечения высокой доступности запросов на чтение. Только для чтения. Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| id | String | Идентификатор, который представляет локальный код, указанный в стандарте ISO 639-1, например `en-US` английский. **Id** для по умолчанию /branding всегда типы `0` строки или `default` . Только для чтения. <br/><br/>**ПРИМЕЧАНИЕ:** Несколько фирменных окей для одного локального уровня в настоящее время не поддерживаются. Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| signInPageText | Строка | Текст, который отображается в нижней части окна для регистрации. С помощью этого можно сообщить дополнительные сведения, например номер телефона в службу поддержки или юридический отчет. Этот текст должен быть unicode и не превышать 1024 символов. Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| squareLogo | Stream | Квадратная версия логотипа вашей компании, которая отображается Windows 10 вне окна (OOBE) и когда Windows автопилот включен для развертывания. Разрешены типы PNG или JPEG размером не более 240 x 240 пикселей и размером не более 10 КБ. Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа. Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Возвращается только с помощью оператора `$select`.|
| squareLogoRelativeUrl | Строка | Относительный URL-адрес для свойства **squareLogo,** который CDN базовый URL-адрес **из cdnList** для предоставления версии, обслуживаемой CDN. Только для чтения. Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| usernameHintText | Строка | Строка, отображаемая в виде подсказки в текстовом ящике имени пользователя на экране входной записи. Этот текст должен быть юникодом без ссылок или кода и не может превышать 64 символов. Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
| локализация | Коллекция [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) | Добавьте другой брендинг на основе локального уровня. |

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organizationalBranding",
  "baseType": "microsoft.graph.organizationalBrandingProperties",
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

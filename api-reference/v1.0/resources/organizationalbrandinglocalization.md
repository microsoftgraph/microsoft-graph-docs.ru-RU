---
title: тип ресурса organizationalBrandingLocalization
description: Содержит сведения о локализации брендинга организации.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 847f5271250de49108dfcb7c680847121ea35063
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647016"
---
# <a name="organizationalbrandinglocalization-resource-type"></a>тип ресурса organizationalBrandingLocalization

Пространство имен: microsoft.graph

Ресурс, поддерживаюющий управление языковым брендингом. Хотя вы не можете изменить язык исходной конфигурации, этот ресурс позволяет создать новую конфигурацию для другого языка.

Наследует от [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Списки организационныхбрандингЛокализации](../api/organizationalbranding-list-localizations.md)|Коллекция [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|Получите список объектов [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) и их свойств.|
|[Создание organizationalBrandingLocalization](../api/organizationalbranding-post-localizations.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|Создайте новый [объект organizationalBrandingLocalization.](../resources/organizationalbrandinglocalization.md)|
|[Получение organizationalBrandingLocalization](../api/organizationalbrandinglocalization-get.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|Ознакомьтесь с свойствами и отношениями объекта [организационнойbrandingLocalization.](../resources/organizationalbrandinglocalization.md)|
|[Обновление organizationalBrandingLocalization](../api/organizationalbrandinglocalization-update.md)| Нет |Обновление свойств объекта [organizationalBrandingLocalization.](../resources/organizationalbrandinglocalization.md)|
|[Удаление organizationalBrandingLocalization](../api/organizationalbrandinglocalization-delete.md)|Нет|Удаляет объект [organizationalBrandingLocalization.](../resources/organizationalbrandinglocalization.md)|

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| backgroundColor | String | Цвет, который будет отображаться на месте фонового изображения в подключениях с низкой пропускной способностью. Рекомендуется использовать основной цвет логотипа баннера или цвета организации. Укажите это в hexadecimal формате, например, белый `#FFFFFF` . Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| backgroundImage | Stream | Изображение, которое отображается в качестве фона страницы регистрации. Допустимые типы PNG или JPEG не меньше 300 КБ и не более 1920 × 1080 пикселей. Меньшее изображение уменьшит требования к пропускной способности и сделает загрузку страницы быстрее. Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| backgroundImageRelativeUrl | String | Относительный URL-адрес свойства **backgroundImage,** который сочетается с базовым URL CDN из **cdnList,** чтобы предоставить версию, обслуживаемую CDN. Только для чтения. Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| bannerLogo | Stream | Баннерная версия логотипа вашей компании, которая отображается на странице входного знака. Допустимые типы PNG или JPEG не более 36 × 245 пикселей. Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа. Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| bannerLogoRelativeUrl | String | Относительный URL-адрес свойства **bannerLogo,** который сочетается с базовым URL-адресом CDN из **cdnList,** чтобы предоставить только для чтения версию, обслуживаемую CDN. Только для чтения. Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| cdnList | Коллекция String | Список базовых URL-адресов для всех CDN поставщиков, обслуживающих активы текущего ресурса. Несколько CDN одновременно используются для обеспечения высокой доступности запросов на чтение. Только для чтения. Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| id | String | Идентификатор, который представляет указанный локальный код с использованием имен культуры. Имена культур следуют стандарту RFC 1766 в формате "languagecode2-country/regioncode2", где "languagecode2" — это код из двух букв более низкого уровня, полученный из ISO 639-1, а "country/regioncode2" — это код с двумя буквами верхнего уровня, полученный из ISO 3166. Например, американский английский язык `en-US` . **Id** для по умолчанию /branding всегда типы `0` строки или `default` . Только для чтения. <br/><br/>**ПРИМЕЧАНИЕ:** Несколько фирменных окей для одного локального уровня в настоящее время не поддерживаются. Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| signInPageText | String | Текст, который отображается в нижней части окна для регистрации. С помощью этого можно сообщить дополнительные сведения, например номер телефона в службу поддержки или юридический отчет. Этот текст должен быть unicode и не превышать 1024 символов. Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| squareLogo | Stream | Квадратная версия логотипа вашей компании, которая отображается Windows 10 вне окна (OOBE) и когда Windows автопилот включен для развертывания. Разрешены типы PNG или JPEG размером не более 240 x 240 пикселей и размером не более 10 КБ. Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа. Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md).|
| squareLogoRelativeUrl | String | Относительный URL-адрес для свойства **squareLogo,** который CDN базовый URL-адрес **из cdnList** для предоставления версии, обслуживаемой CDN. Только для чтения. Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| usernameHintText | String | Строка, отображаемая в виде подсказки в текстовом ящике имени пользователя на экране входной записи. Этот текст должен быть юникодом без ссылок или кода и не может превышать 64 символов. Наследуется [от organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |

## <a name="relationships"></a>Отношения
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
  "usernameHintText": "String"
}
```

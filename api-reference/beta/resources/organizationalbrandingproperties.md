---
title: тип ресурса organizationalBrandingProperties
description: Содержит сведения о брендинге организации.
localization_priority: Normal
author: almars
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f68c33e7a3cf81e5d3debedcd6162ec59ddcce03
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266824"
---
# <a name="organizationalbrandingproperties-resource-type"></a>тип ресурса organizationalBrandingProperties

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
>Чтобы добавить настраиваемый брендинг, необходимо использовать Azure Active Directory Premium 1, Premium 2 или Basic или иметь лицензию Microsoft 365. Дополнительные сведения о лицензировании и выпусках см. в документе [Sign up for Azure AD Premium.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium)<br><br>Выпуски Azure AD Premium и Basic доступны для клиентов в Китае с помощью всемирного экземпляра Azure Active Directory. В настоящее время выпуски Azure AD Premium и Basic не поддерживаются в службе Azure, выполняемой 21Vianet в Китае. Дополнительные сведения можно получить с помощью [форума Azure Active Directory.](https://feedback.azure.com/forums/169401-azure-active-directory/)

Содержит сведения о брендинге организации.

Организации могут настраивать страницы регистрации Azure AD, которые отображаются при входе пользователей в конкретные приложения своей организации или когда Azure AD идентифицирует клиента пользователя из имени пользователя. Разработчик также может ознакомиться с информацией о брендинге компании и настроить интерфейс приложения, чтобы настроить его специально для пользователя, вписаного в нее, с помощью фирменого бренда.

Компании могут добавлять различные брендинги в зависимости от локального уровня. Locale служит ключом во всех запросах.

>**Примечание:** Брендинг выставляется как свойство под организацией с коллекцией локализации, определенной для локального. **organizationalBrandingProperties** — это абстрактный класс, определяющий свойства **для organizationalBranding.**

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание](../api/organizationalbrandingproperties-create.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | Создание организационного брендинга с помощью объекта organizationalBrandingProperties. |
| [получение](../api/organizationalbrandingproperties-get.md); | [organizationalBrandingProperties](organizationalbrandingproperties.md) | Чтение свойств и связей объекта organizationalBrandingProperties. |
| [Обновление](../api/organizationalbrandingproperties-update.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | Обновление объекта organizationalBrandingProperties. |
| [удаление](../api/organizationalbrandingproperties-delete.md); | Нет | Удаление объекта organizationalBrandingProperties. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|backgroundColor|Строка| Цвет, который будет отображаться на месте фонового изображения в подключениях с низкой пропускной способностью. Здесь рекомендуется использовать основной цвет логотипа баннера или цвета организации. Укажите это в hexadecimal (например, белый #FFFFFF). |
|backgroundImage|Stream| Изображение, которое отображается в качестве фона знака на странице. .png или .jpg не больше 1920x1080 и меньше 300kb. Меньшее изображение уменьшит требования к пропускной способности и сделает загрузку страниц более высокой. |
|bannerLogo|Stream| На странице входного знака отображается баннерная версия логотипа вашей компании. .png или .jpg не превышает 36x245px. Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа. |
|id|Строка| Это id, унаследованный от microsoft.graph.entity, — это локал, указывающий стандарт ISO 639 для языка, например английский — "en-ru" или "ru". Если мы обналичим функциональность с несколькими фирменными марками для одного локального уровня, это можно изменить. Обратите внимание, что id для default/branding всегда является "und" до тех пор, пока у нас нет однотонов без ключей. Только для чтения. |
|signInPageText|Строка| Текст, который отображается в нижней части окна для регистрации. С помощью этого можно сообщить дополнительные сведения, например номер телефона в службу поддержки или юридический отчет. Этот текст должен быть unicode и не превышать 1024 символов. |
|squareLogo|Stream| Квадратная версия логотипа вашей компании. Это отображается в windows 10 вне окна (OOBE) опытом и когда Windows Автопилот включен для развертывания. .png или .jpg размером не более 240x240px и не более 10 кб. Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа. |
|usernameHintText|Строка| Строка, отображаемая в виде подсказки в текстовом ящике имени пользователя на экране знака. Этот текст должен быть Unicode без ссылок или кода и не может превышать 64 символов. |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizationalBrandingProperties",
  "keyProperty": "id"
}-->

```json
{
  "backgroundColor": "String",
  "backgroundImage": "Stream",
  "bannerLogo": "Stream",
  "id": "String (identifier)",
  "signInPageText": "String",
  "squareLogo": "Stream",
  "usernameHintText": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organizationalBrandingProperties resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

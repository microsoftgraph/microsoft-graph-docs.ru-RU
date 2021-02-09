---
title: Тип ресурса organizationalBrandingProperties
description: Содержит сведения о фирменой фирменой марке организации.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 531e026fa08e13bafc72f0bf361345e7f1d10c0a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158333"
---
# <a name="organizationalbrandingproperties-resource-type"></a>Тип ресурса organizationalBrandingProperties

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
>Для добавления пользовательской фирменной настройки необходимо использовать выпуски Azure Active Directory Premium 1, Premium 2 или Basic или лицензию на Microsoft 365. Дополнительные сведения о лицензировании и выпусках см. в подписке [на Azure AD Premium.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium)<br><br>Выпуски Azure AD Premium и Basic доступны для клиентов в Китае с помощью всемирного экземпляра Azure Active Directory. Выпуски Azure AD Premium и Basic в настоящее время не поддерживаются в службе Azure под управлением 21Vianet в Китае. Дополнительные сведения можно найти на форуме [Azure Active Directory.](https://feedback.azure.com/forums/169401-azure-active-directory/)

Содержит сведения о фирменой фирменой марке организации.

Организации могут настраивать свои страницы для входов в Azure AD, которые отображаются при входе пользователей в приложения, определенные в клиенте организации, или когда Azure AD идентифицирует клиент пользователя по имени пользователя. Разработчик также может прочитать сведения о фирменой фирменой марке компании и настроить интерфейс приложения, чтобы адаптировать его специально для во выписаного пользователя с использованием фирменой марки компании.

Компании могут добавлять разные фирменные фирменки на основе региональных региональных ний. Региональные органы служат ключом во всех запросах.

>**Примечание.** Фирменное название является свойством организации с коллекцией локализации, специфичная для конкретных региональных стандартов. **organizationalBrandingProperties** — это абстрактный класс, который определяет свойства **для organizationalBranding.**

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание](../api/organizationalbrandingproperties-create.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | Создайте фирменую марку организации с помощью объекта organizationalBrandingProperties. |
| [Получение](../api/organizationalbrandingproperties-get.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | Чтение свойств и связей объекта organizationalBrandingProperties. |
| [Обновление](../api/organizationalbrandingproperties-update.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | Обновление объекта organizationalBrandingProperties. |
| [удаление](../api/organizationalbrandingproperties-delete.md); | Нет | Удаление объекта organizationalBrandingProperties. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|backgroundColor|String| Цвет, который будет отображаться на месте фонового изображения в подключениях с низкой пропускной способностью. Здесь рекомендуется использовать основной цвет логотипа баннера или цвета организации. Укажите это в hexadecimal (например, белый #FFFFFF). |
|backgroundImage|Stream| Изображение, которое отображается в качестве фона страницы для регистрации. .png или JPG не больше 1920x1080 и меньше 300 кб. Меньшее изображение уменьшит требования к пропускной способности и сделает загрузку страниц более высокой. |
|bannerLogo|Stream| На странице для регистрации появится баннер с логотипом вашей компании. .png или JPG не больше 36x245px. Мы рекомендуем использовать прозрачное изображение без заполнения логотипа. |
|id|String| Это ид, наследуемый от microsoft.graph.entity, это языковой стандарт, определяющий стандарт ISO 639 для языка, например английский — "en-us" или "en". В будущем, если функции будут иметь несколько фирменной фирменной марки для одного локали, это можно изменить. Обратите внимание, что ид для default /branding всегда является "und", пока у нас не будет singleton-элементов без ключей. Только для чтения. |
|signInPageText|String| Текст, который отображается в нижней части окна для регистрации. С его помощью можно сообщить дополнительную информацию, например номер телефона, в службу поддержки или в юридический отчет. Этот текст должен быть Юникод и не должен превышать 1024 символов. |
|squareLogo|Stream| Квадратная версия логотипа компании. Эта возможность отображается в windows 10 при включаемом (OOBE) режиме и когда Windows Autopilot включен для развертывания. PNG или JPG размером не более 240x240px и размером не более 10 кб. Мы рекомендуем использовать прозрачное изображение без заполнения логотипа. |
|usernameHintText|String| Строка, отображаемая в виде подсказки в текстовом ящике имени пользователя на экране входов. Этот текст должен быть Юникод без ссылок и кода и не может превышать 64 символа. |

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

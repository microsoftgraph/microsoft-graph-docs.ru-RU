---
title: Тип ресурса certificateBasedAuthConfiguration
description: Представляет коллекцию сертификатов.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0fcc5f37cb55ad0cc5e9e76bf0fe7efb6c4ab517
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153482"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a>Тип ресурса certificateBasedAuthConfiguration

Пространство имен: microsoft.graph

Проверка подлинности на основе сертификатов позволяет azure Active Directory проверить подлинность с помощью сертификата клиента на устройстве с Windows, Android или iOS при подключении учетной записи Exchange Online к:

- Мобильные приложения Майкрософт, такие как Outlook и Word
- Exchange ActiveSync (EAS)

Настройка этой функции устраняет необходимость ввода имени пользователя и пароля в определенных почтовых Microsoft Office приложениях на мобильном устройстве.

Конфигурация проверки подлинности на основе сертификатов предоставляется с помощью коллекции сертификатных органов. Эти органы используются для создания надежной цепочки сертификатов, которая позволяет клиентам аутентификацию с помощью Azure Active Directory с помощью сертификата клиента.

Узнайте больше о проверке подлинности на [основе сертификатов в Azure Active Directory.](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-list.md) | [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) | Список свойств коллекции **certificateBasedAuthConfiguration.** |
| [Создание certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) | Создание объекта **certificateBasedAuthConfiguration.** |
| [Get certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-get.md) | [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) | Чтение свойств объекта **certificateBasedAuthConfiguration.** |
| [Удаление certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-delete.md) | Нет | Удаление объекта **certificateBasedAuthConfiguration.** |

>[!NOTE]
>Обновление **certificateBasedAuthConfiguration** не поддерживается. Чтобы изменить **certificateBasedAuthConfiguration,** сначала удалите, а затем создайте **новый certificateBasedAuthConfiguration.**

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|certificateAuthorities|[Коллекция certificateAuthority](certificateauthority.md)|Коллекция органов сертификации, создав цепочку доверенных сертификатов.|
|id|String|Уникальный идентификатор конфигурации auth на основе сертификата. Только для чтения.|

## <a name="relationships"></a>Связи

Нет,

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration",
  "keyProperty": "id"
}-->

```json
{
  "certificateAuthorities": {"@odata.type": "collection(microsoft.graph.certificateAuthority)"},
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "certificateBasedAuthConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

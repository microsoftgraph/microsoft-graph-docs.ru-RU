---
title: тип ресурса certificateBasedAuthConfiguration
description: Представляет коллекцию органов сертификации.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 8580851fe5f2c9266659b0bf26e85a9eca07185c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443904"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a>тип ресурса certificateBasedAuthConfiguration

Пространство имен: microsoft.graph

Проверка подлинности на основе сертификатов позволяет проверить подлинность в Azure Active Directory с клиентской сертификатом на устройстве Windows, Android или iOS при подключении учетной записи Exchange Online к:

- Мобильные приложения Майкрософт, такие как Outlook и Word
- Exchange ActiveSync (EAS)

Настройка этой функции исключает необходимость ввода имени пользователя и сочетания паролей в определенные почтовые и Microsoft Office приложения на мобильном устройстве.

Конфигурация проверки подлинности на основе сертификатов предоставляется через коллекцию органов сертификации. Органы сертификации используются для создания цепочки доверенных сертификатов, которая позволяет клиентам быть аутентификацией в Azure Active Directory с помощью клиентского сертификата.

Узнайте больше о проверке подлинности на основе [сертификатов в Azure Active Directory.](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [List certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-list.md) | [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) | Список свойств коллекции **certificateBasedAuthConfiguration.** |
| [Создание certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) | Создайте новый **объект certificateBasedAuthConfiguration.** |
| [Получить certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-get.md) | [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) | Ознакомьтесь с свойствами **объекта certificateBasedAuthConfiguration.** |
| [Удаление certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-delete.md) | Нет | Удаление **объекта certificateBasedAuthConfiguration.** |

>[!NOTE]
>Обновление **certificateBasedAuthConfiguration** не поддерживается. Чтобы изменить **certificateBasedAuthConfiguration,** сначала удалите, а затем создайте новый **сертификатBasedAuthConfiguration**.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|certificateAuthorities|[коллекция certificateAuthority](certificateauthority.md)|Коллекция органов сертификации, создав цепочку надежных сертификатов.|
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

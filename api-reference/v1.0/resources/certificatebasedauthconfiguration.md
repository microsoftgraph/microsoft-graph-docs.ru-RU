---
title: тип ресурса certificateBasedAuthConfiguration
description: Представляет коллекцию органов сертификации.
ms.localizationpriority: medium
author: adimitui
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 53e56f78508131e3a08e7896095a7f986346fba2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104259"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a>тип ресурса certificateBasedAuthConfiguration

Пространство имен: microsoft.graph

Проверка подлинности на основе сертификатов позволяет Azure Active Directory с помощью клиентского сертификата на устройстве Windows, Android или iOS при подключении учетной записи Exchange Online к:

- Мобильные приложения Майкрософт, такие как Outlook и Word
- клиентам Exchange ActiveSync (EAS).

Настройка этой функции исключает необходимость ввода имени пользователя и сочетания паролей в определенные почтовые и Microsoft Office приложения на мобильном устройстве.

Конфигурация проверки подлинности на основе сертификатов предоставляется через коллекцию органов сертификации. Органы сертификации используются для создания цепочки доверенных сертификатов, которая позволяет клиентам Azure Active Directory с клиентской сертификатом.

Дополнительные информацию о проверке подлинности на основе сертификатов в [Azure Active Directory.](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)

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
|id|Строка|Уникальный идентификатор конфигурации auth на основе сертификата. Только для чтения.|

## <a name="relationships"></a>Отношения

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

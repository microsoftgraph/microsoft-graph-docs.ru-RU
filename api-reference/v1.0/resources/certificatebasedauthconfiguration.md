---
title: Тип ресурса Цертификатебаседаусконфигуратион
description: Представляет коллекцию центров сертификации.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d0b5b57a7594dfaf4fde88615c6a21314618c0eb
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539290"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a>Тип ресурса Цертификатебаседаусконфигуратион

Проверка подлинности на основе сертификатов обеспечивает проверку подлинности Azure Active Directory с помощью сертификата клиента на устройстве Windows, Android или iOS при подключении учетной записи Exchange Online к:

- Мобильные приложения Майкрософт, такие как Outlook и Word
- Клиенты Exchange ActiveSync (EAS)

Настройка этой функции исключает необходимость ввода имени пользователя и пароля в определенные приложения электронной почты и приложения Microsoft Office на мобильном устройстве.

Настройка проверки подлинности на основе сертификатов обеспечивается через коллекцию центров сертификации. Центры сертификации используются для установки доверенной цепочки сертификатов, что позволяет клиентам выполнять проверку подлинности с помощью Azure Active Directory с помощью сертификата клиента.

Узнайте больше о [проверке подлинности на основе сертификатов в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Цертификатебаседаусконфигуратион](../api/certificatebasedauthconfiguration-list.md) | [цертификатебаседаусконфигуратион](certificatebasedauthconfiguration.md) | Перечисление свойств коллекции **цертификатебаседаусконфигуратион** . |
| [Создание Цертификатебаседаусконфигуратион](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [цертификатебаседаусконфигуратион](certificatebasedauthconfiguration.md) | Создание нового объекта **цертификатебаседаусконфигуратион** . |
| [Получение Цертификатебаседаусконфигуратион](../api/certificatebasedauthconfiguration-get.md) | [цертификатебаседаусконфигуратион](certificatebasedauthconfiguration.md) | Чтение свойств объекта **цертификатебаседаусконфигуратион** . |
| [Удаление Цертификатебаседаусконфигуратион](../api/certificatebasedauthconfiguration-delete.md) | Нет | Удаление объекта **цертификатебаседаусконфигуратион** . |

>[!NOTE]
>Обновление **церфикатебаседаусконфигуратион** не поддерживается. Чтобы изменить **церфикатебаседаусконфигуратион**, сначала удалите его, а затем создайте новый **церфикатебаседаусконфигуратион**.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|цертификатеаусоритиес|Коллекция [цертификатеаусорити](certificateauthority.md)|Коллекция центров сертификации, которая создает доверенную цепочку сертификатов.|
|id|String|Уникальный идентификатор конфигурации проверки подлинности на основе сертификатов. Только для чтения.|

## <a name="relationships"></a>Отношения

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration",
  "baseType": "",
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

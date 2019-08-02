---
title: Тип ресурса Феатурероллаутполици
description: Представляет политику развертывания компонентов, связанную с объектом каталога.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 50d54ae046ef5a0283f5eb2e474fd0faab781687
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062180"
---
# <a name="featurerolloutpolicy-resource-type"></a>Тип ресурса Феатурероллаутполици

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику развертывания компонентов, связанную с объектом каталога. Создание политики развертывания компонентов поможет администраторам клиентов пилотно использовать определенную группу перед включением функций для всей Организации. Это минимизирует воздействие и помогает администраторам постепенно тестировать и отменять связанные функции проверки подлинности.

Ниже приведены ограничения на развертывание функций.

- Каждая функция поддерживает не более 10 групп.
- Поле **appliesTo** поддерживает только группы.
- Динамические группы и вложенные группы не поддерживаются.

Ниже приведены предварительные требования для каждой из функций, которые в настоящее время супортед для развертывания с помощью этой политики развертывания.

### <a name="passthrough-authentication"></a>Сквозная проверка подлинности

* Определите сервер под управлением Windows Server 2012 R2 или более поздней версии, на котором нужно запустить агент [пасссраугхаусентикатион](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-pta) .Убедитесь, что сервер присоединен к домену, может выполнять проверку подлинности выбранных пользователей с помощью Active Directory и может связываться с Azure AD на исходящих портах/URL-адресах.
* [Скачайте](https://aka.ms/getauthagent) & установить агент проверки подлинности Microsoft Azure AD Connect на сервере.
* Чтобы обеспечить высокий уровень доступности, установите дополнительные агенты проверки подлинности на других серверах, как описано [здесь](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).
* Убедитесь, что параметры [интеллектуальной блокировки](https://docs.microsoft.com/en-us/azure/active-directory/authentication/howto-password-smart-lockout) настроены соответствующим образом. Это необходимо для того, чтобы локальные учетные записи пользователей Active Directory не блокировались с помощью недопустимых субъектов.

### <a name="seamlesssso"></a>Сеамлессссо

* Включите [сеамлессссо](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-sso) для лесов Active Directory в соответствии с [этими](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) инструкциями.

### <a name="passwordhashsync"></a>Пассвордхашсинк

* Включите [пассвордхашсинк](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/whatis-phs) на странице "дополнительные компоненты" в Azure AD Connect.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список ФеатурероллаутполиЦиес](../api/directory-list-featurerolloutpolicies.md) | [Феатурероллаутполици](featurerolloutpolicy.md) | Получение списка объектов Феатурероллаутполици. |
| [Получение Феатурероллаутполици](../api/featurerolloutpolicy-get.md) | [Феатурероллаутполици](featurerolloutpolicy.md) | Получение свойств и связей объекта феатурероллаутполици. ||
| [Создание Феатурероллаутполици](../api/directory-post-featurerolloutpolicies.md) | [Феатурероллаутполици](featurerolloutpolicy.md) | Создание нового объекта Феатурероллаутполици.
| [Обновление Феатурероллаутполици](../api/featurerolloutpolicy-update.md) | [Феатурероллаутполици](featurerolloutpolicy.md) | Обновление свойств объекта феатурероллаутполици. |
| [Удаление Феатурероллаутполици](../api/featurerolloutpolicy-delete.md) | Нет | Удаление объекта Феатурероллаутполици. |
| [Назначение appliesTo](../api/featurerolloutpolicy-post-appliesto.md) | [directoryObject](directoryobject.md) | Назначение directoryObject для развертывания компонентов. |
| [Удаление appliesTo](../api/featurerolloutpolicy-delete-appliesto.md) | Нет | Удаление directoryObject из развертывания компонента. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|String|Описание этой политики развертывания функций.|
|displayName|Строка|Отображаемое имя для этой политики развертывания компонента.|
|состав|Стажедфеатуренаме| Возможные значения: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.|
|id|String| Только для чтения.|
|Исапплиедтурганизатион|Boolean|Указывает, следует ли применять эту политику развертывания функций ко всей Организации.|
|isEnabled|Boolean|Указывает, включен ли выпуск компонентов.|

## <a name="relationships"></a>Отношения

| Отношение | Тип        | Описание |
|:-------------|:------------|:------------|
|Тег|Коллекция [directoryObject](directoryobject.md)| Допускается значение null. Указывает список Директорйобжектс, для которых включена функция.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "feature": "string",
  "id": "String (identifier)",
  "isAppliedToOrganization": false,
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "featureRolloutPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

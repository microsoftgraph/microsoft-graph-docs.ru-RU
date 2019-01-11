---
title: Тип ресурса governancePermission
description: 'Представляет, governanceSubject имеет разрешение на доступ к определенным governanceResource.  '
localization_priority: Normal
ms.openlocfilehash: e082ca50e5642e865b3e30859eea607df63a03b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882875"
---
# <a name="governancepermission-resource-type"></a>Тип ресурса governancePermission

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет, [governanceSubject](../resources/governancesubject.md) имеет разрешение на доступ к определенным [governanceResource](../resources/governanceresource.md).  


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|accessLevel|Строка|Уровень доступа. Допустимые значения: ``None``, ``UserRead``, ``AdminRead``, и ``AdminReadWrite``.|
|isActive|Логический|Указывает, если инициатора запроса имеет назначения активная роль на уровне доступа.|
|isEligible|Логический|Указывает, имеет ли инициатора запроса все назначения ролей право на уровне доступа.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```

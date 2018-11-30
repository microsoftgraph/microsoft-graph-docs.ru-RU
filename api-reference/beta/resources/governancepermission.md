---
title: Тип ресурса governancePermission
description: 'Представляет, governanceSubject имеет разрешение на доступ к определенным governanceResource.  '
ms.openlocfilehash: d7b3e1eb70c89c278ccc2a8b3e9a16e265e4ae97
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079406"
---
# <a name="governancepermission-resource-type"></a>Тип ресурса governancePermission

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет, [governanceSubject](../resources/governancesubject.md) имеет разрешение на доступ к определенным [governanceResource](../resources/governanceresource.md).  


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|accessLevel|String|Уровень доступа. Допустимые значения: ``None``, ``UserRead``, ``AdminRead``, и ``AdminReadWrite``.|
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
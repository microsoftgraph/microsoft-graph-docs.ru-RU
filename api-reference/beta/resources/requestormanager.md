---
title: сложный тип Рекуесторманажер
description: Определяет связь с другим пользователем в клиенте, который будет разрешен в качестве утверждающего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ca8559d3ecf7ba4110a7e2871f8e6acf545d2906
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581154"
---
# <a name="requestormanager-complex-type"></a>сложный тип Рекуесторманажер

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в [параметрах утверждения политики назначения пакетов Access](accesspackageassignmentpolicy.md). Это подтип набора [пользователей](userset.md), в котором `@odata.type` значение указывает на то `#microsoft.graph.requestorManager` , что руководитель запрашивающего пользователя должен быть утверждающим.  При создании этапа утверждения политики назначения пакетов Access с Рекуесторманажер также включает другой утверждающий, например одного пользователя или члена группы, если у запрашивающего пользователя нет руководителя.


## <a name="properties"></a>Свойства


| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| Создание резервной копии | Логический | Для руководителя на этапе утверждения указывает, является ли руководитель резервным утверждающим. |
|манажерлевел | Int32 | Иерархический уровень руководителя по отношению к запрашивающему. Например, непосредственный менеджер запрашивающего Манажерлевел должен иметь значение 1, в то время как руководитель запрашивающего менеджера будет иметь Манажерлевел 2. Значение по умолчанию для Манажерлевел — 1. Возможные значения этого свойства находятся в диапазоне от 1 до 2. |


## <a name="json-representation"></a>Представление JSON

Ниже представлено представление типа в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorManager",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "isBackup": false,
  "managerLevel": 1
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requestorManager complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



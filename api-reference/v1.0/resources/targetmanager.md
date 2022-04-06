---
title: тип ресурса targetManager
description: Сложный тип для управления правами, чтобы указать диспетчера, в том числе косвенные менеджеры пользователя, могут запрашивать от имени этого пользователя.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 06859aea4cc966ca25ded6dc8e972adf6ca2a600
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608388"
---
# <a name="targetmanager-complex-type"></a>сложный тип targetManager

Пространство имен: microsoft.graph

Этот тип, используемый в политике назначения пакетов доступа, наследуется из [subjectSet](../resources/subjectset.md) и указывает диспетчеру, в том числе непрямые менеджеры пользователя, которые могут запрашивать от имени этого пользователя.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|managerLevel|Int32|Уровень диспетчера от 1 до 4. Прямой диспетчер — 1.|

## <a name="relationships"></a>Связи
Отсутствуют.
## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.targetManager"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetManager",
  "managerLevel": "Integer"
}
```



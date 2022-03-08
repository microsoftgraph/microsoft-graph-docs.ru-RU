---
title: тип ресурса customExtensionHandlerInstance
description: Используется для записи состояния пользовательского экземпляра расширения рабочего процесса, запускаемого по запросу назначения пакета доступа.
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d832ca092404eb3221952b0b46b720d8f0c217cc
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339287"
---
# <a name="customextensionhandlerinstance-resource-type"></a>тип ресурса customExtensionHandlerInstance

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для записи состояния экземпляра расширения пользовательского  [рабочего](customaccesspackageworkflowextension.md) процесса, запускаемого по запросу назначения [пакета доступа](accesspackageassignmentrequest.md).

## <a name="methods"></a>Методы
Нет

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|customExtensionId|Строка|Идентификатор [настраиваемогоAccessPackageWorkflowExtension](customaccesspackageworkflowextension.md) , срабатываемого в этом экземпляре.|
|externalCorrelationId|Строка|Уникальный ID запуска для приложения логики.|
|этап|accessPackageCustomExtensionStage|Указывает этап рабочего процесса запроса при запуске настраиваемого расширения пакета доступа. Возможные значения: `assignmentRequestCreated`, `assignmentRequestApproved`, `assignmentRequestGranted`, `assignmentRequestRemoved`, `assignmentFourteenDaysBeforeExpiration`, `assignmentOneDayBeforeExpiration`, `unknownFutureValue`.|
|status|accessPackageCustomExtensionHandlerStatus|Состояние запроса для запуска пользовательского рабочего процесса расширения пакета доступа, связанного с логическим приложением. Допустимые значения: `requestSent`, `requestReceived`, `unknownFutureValue`.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customExtensionHandlerInstance"
}
-->
``` json

{
  "@odata.type": "#microsoft.graph.customExtensionHandlerInstance",
  "stage": "String",
  "customExtensionId": "String",
  "externalCorrelationId": "String",
  "status": "String"
}
```


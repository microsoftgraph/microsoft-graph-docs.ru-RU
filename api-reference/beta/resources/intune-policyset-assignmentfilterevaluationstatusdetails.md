---
title: Тип ресурса assignmentFilterEvaluationStatusDetails
description: Класс, содержащий сведения о полезной нагрузке, к которой применен фильтр.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4b569b59ad929c0928edecb90c7ef05432fbc082
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160908"
---
# <a name="assignmentfilterevaluationstatusdetails-resource-type"></a>Тип ресурса assignmentFilterEvaluationStatusDetails

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий сведения о полезной нагрузке, к которой применен фильтр.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список assignmentFilterEvaluationStatusDetailses](../api/intune-policyset-assignmentfilterevaluationstatusdetails-list.md)|[Коллекция assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)|Список свойств и связей объектов [assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)|
|[Get assignmentFilterEvaluationStatusDetails](../api/intune-policyset-assignmentfilterevaluationstatusdetails-get.md)|[assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)|Чтение свойств и связей объекта [assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)|
|[Создание assignmentFilterEvaluationStatusDetails](../api/intune-policyset-assignmentfilterevaluationstatusdetails-create.md)|[assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)|Создание объекта [assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)|
|[Удаление assignmentFilterEvaluationStatusDetails](../api/intune-policyset-assignmentfilterevaluationstatusdetails-delete.md)|Нет|Удаляет [assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)|
|[Обновление assignmentFilterEvaluationStatusDetails](../api/intune-policyset-assignmentfilterevaluationstatusdetails-update.md)|[assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)|Обновление свойств объекта [assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта AssignmentFilterEvaluationStatusDetails.|
|payloadId|String|PayloadId, к которому применен фильтр.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.assignmentFilterEvaluationStatusDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationStatusDetails",
  "id": "String (identifier)",
  "payloadId": "String"
}
```





---
title: Тип ресурса deviceManagement
description: Singleton, который выступает в качестве контейнера для коллекции сущностей UserPFXCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d87095f5840867223830fb1f778a9fadce747b36
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752024"
---
# <a name="devicemanagement-resource-type"></a>Тип ресурса deviceManagement

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Singleton, который выступает в качестве контейнера для коллекции сущностей UserPFXCertificate.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceManagement](../api/intune-raimportcerts-devicemanagement-get.md)|[deviceManagement](../resources/intune-raimportcerts-devicemanagement.md)|Чтение свойств и связей объекта [deviceManagement](../resources/intune-raimportcerts-devicemanagement.md).|
|[Обновление объекта deviceManagement](../api/intune-raimportcerts-devicemanagement-update.md)|[deviceManagement](../resources/intune-raimportcerts-devicemanagement.md)|Обновление свойств объекта [deviceManagement](../resources/intune-raimportcerts-devicemanagement.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Н/Д|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```





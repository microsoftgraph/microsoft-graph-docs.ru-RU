---
title: Тип ресурса deviceManagement
description: Singleton, который выступает в качестве контейнера для коллекции сущностей UserPFXCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e860bb52cccb16ccca2e90a3a61631e6d1c00611
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60449575"
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




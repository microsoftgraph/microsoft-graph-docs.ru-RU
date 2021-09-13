---
title: Тип ресурса deviceManagement
description: Singleton, который выступает в качестве контейнера для коллекции сущностей UserPFXCertificate.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 580b837298d7fcbb7bd839f4e2837a704f2c01c2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044498"
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

## <a name="relationships"></a>Отношения
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





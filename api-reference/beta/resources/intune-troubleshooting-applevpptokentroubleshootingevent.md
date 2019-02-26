---
title: Тип ресурса Апплевпптокентраублешутинжевент
description: Событие, представляющее событие устранения неполадок маркера Apple VPP.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 13459e2d8f76111137014918246fe1a573a191cd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160468"
---
# <a name="applevpptokentroubleshootingevent-resource-type"></a>Тип ресурса Апплевпптокентраублешутинжевент

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Событие, представляющее событие устранения неполадок маркера Apple VPP.


Наследуется от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Апплевпптокентраублешутинжевентс](../api/intune-troubleshooting-applevpptokentroubleshootingevent-list.md)|Коллекция [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)|Список свойств и связей объектов [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .|
|[Получение Апплевпптокентраублешутинжевент](../api/intune-troubleshooting-applevpptokentroubleshootingevent-get.md)|[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)|Чтение свойств и связей объекта [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .|
|[Создание Апплевпптокентраублешутинжевент](../api/intune-troubleshooting-applevpptokentroubleshootingevent-create.md)|[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)|Создание нового объекта [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .|
|[Удаление Апплевпптокентраублешутинжевент](../api/intune-troubleshooting-applevpptokentroubleshootingevent-delete.md)|Нет|Удаляет объект [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md).|
|[Обновление Апплевпптокентраублешутинжевент](../api/intune-troubleshooting-applevpptokentroubleshootingevent-update.md)|[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)|Обновление свойств объекта [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).|
|eventDateTime|DateTimeOffset|Время возникновения события. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).|
|correlationId|String|Идентификатор, используемый для трассировки сбоя в службе. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).|
|Траублешутинжеррордетаилс|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|Объект, содержащий подробные сведения об ошибке и ее исправлении. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).|
|eventName|String|Имя события, соответствующее соБытию устранения неполадок. Это неОбязательное поле, унаследованное от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|Аддитионалинформатион|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Набор пар строкового ключа и строкового значения, предоставляющий дополнительные сведения о событии устранения неполадок, наСледуемом от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|Токенид|String|Идентификатор токена Apple Volume Purchase Program.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appleVppTokenTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleVppTokenTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "String",
    "failure": "String",
    "failureDetails": "String",
    "remediation": "String",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "String",
        "link": "String"
      }
    ]
  },
  "eventName": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "tokenId": "String"
}
```





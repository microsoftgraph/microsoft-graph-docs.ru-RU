---
title: Тип ресурса Впптокенревокелиценсесактионресулт
description: Состояние действия отзыва лицензий, выполняемого в токене Apple Volume Purchase Program.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d2ec896504435c644767af1ff04a74f4eaf4aa17
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42777504"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a>Тип ресурса Впптокенревокелиценсесактионресулт

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние действия отзыва лицензий, выполняемого в токене Apple Volume Purchase Program.


Наследуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actionName|String|Имя действия наследуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Состояние действия, унаследованного от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md). Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|startDateTime|DateTimeOffset|Время начала действия, унаследованное от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)|
|lastUpdatedDateTime|DateTimeOffset|Время последнего обновления состояния действия, унаследованного от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)|
|тоталлиценсескаунт|Int32|Число неудачных попыток отзыва лицензий.|
|фаиледлиценсескаунт|Int32|Количество лицензий, которые не удалось отозвать.|
|актионфаилуререасон|[впптокенактионфаилуререасон](../resources/intune-shared-vpptokenactionfailurereason.md)|Причина сбоя действия "отзыв лицензий". Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenRevokeLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String"
}
```




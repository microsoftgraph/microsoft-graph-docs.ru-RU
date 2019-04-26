---
title: Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори
description: Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbbf575c7eaecb93e0256d6f672d0c4d6bdd0edf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570042"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a>Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.


НаСледуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Оккурренцедатетиме|DateTimeOffset|Время возникновения элемента журнала. НаСледуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)|
|Рунстате|[Рунстате](../resources/intune-shared-runstate.md)|Состояние элемента. Возможные значения: `unknown`, `success`, `fail`.|
|errorCode|String|Код ошибки для сбоя, пустой при отсутствии ошибки.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory",
  "occurrenceDateTime": "String (timestamp)",
  "runState": "String",
  "errorCode": "String"
}
```




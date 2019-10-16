---
title: Тип ресурса Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус
description: Содержит свойства для состояния развертывания дополнительной политики Виндовсдефендераппликатионконтрол для устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e10728bba5048b1e46889c178710b79043622624
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538842"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-resource-type"></a>Тип ресурса Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для состояния развертывания дополнительной политики Виндовсдефендераппликатионконтрол для устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатусес](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-list.md)|Коллекция [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Список свойств и связей объектов [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .|
|[Получение Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-get.md)|[виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Чтение свойств и связей объекта [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .|
|[Создание Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-create.md)|[виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Создание нового объекта [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .|
|[Удаление Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-delete.md)|Нет|Удаляет объект [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md).|
|[Обновление Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-update.md)|[виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Обновление свойств объекта [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|deviceName|String|Имя устройства.|
|deviceId|String|ИДЕНТИФИКАТОР устройства.|
|lastSyncDateTime|DateTimeOffset|Дата и время последней синхронизации.|
|osVersion|String|Версия ОС Windows.|
|osDescription|String|Описание версии ОС Windows.|
|деплойментстатус|[виндовсдефендераппликатионконтролсупплементалполицистатусес](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses.md)|Состояние развертывания политики. Возможные значения: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.|
|userName|String|Имя пользователя этого устройства.|
|userPrincipalName|String|Имя участника пользователя.|
|полициверсион|String|Доступная для человека версия дополнительной политики Виндовсдефендераппликатионконтрол.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|policy|[виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|Ссылка навигации на дополнительную политику Виндовсдефендераппликатионконтрол.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "osVersion": "String",
  "osDescription": "String",
  "deploymentStatus": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "policyVersion": "String"
}
```




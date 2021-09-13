---
title: тип ресурса windowsDefenderApplicationControlSupplementalPolicy
description: Пока не задокументировано.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e20f4c9a868d842f5de915f1491d2a9f4428888e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039016"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicy-resource-type"></a>тип ресурса windowsDefenderApplicationControlSupplementalPolicy

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsDefenderApplicationControlSupplementalPolicies](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-list.md)|[коллекция windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|Список свойств и связей объектов [WindowsDefenderApplicationControlSupplementalPolicy.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|
|[Get windowsDefenderApplicationControlSupplementalPolicy](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-get.md)|[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|Чтение свойств и связей [объекта WindowsDefenderApplicationControlSupplementalPolicy.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|
|[Создание windowsDefenderApplicationControlSupplementalPolicy](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-create.md)|[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|Создайте [новый объект WindowsDefenderApplicationControlSupplementalPolicy.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|
|[Удаление windowsDefenderApplicationControlSupplementalPolicy](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-delete.md)|Нет|Удаляет [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md).|
|[Обновление windowsDefenderApplicationControlSupplementalPolicy](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-update.md)|[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|Обновление свойств объекта [WindowsDefenderApplicationControlSupplementalPolicy.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|
|[Действие assign](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ для дополнительной политики WindowsDefenderApplicationControl.|
|displayName|String|Отображение имени дополнительной политики WindowsDefenderApplicationControl.|
|description|String|Описание дополнительной политики WindowsDefenderApplicationControl.|
|содержимое|В двоичном формате|Контент дополнительной политики WindowsDefenderApplicationControl в формате byte array.|
|contentFileName|String|Имя файла дополнительного контента политики WindowsDefenderApplicationControl.|
|version|String|Версия дополнительной политики WindowsDefenderApplicationControl.|
|creationDateTime|DateTimeOffset|Дата и время отправки дополнительной политики WindowsDefenderApplicationControl.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения политики дополнительных приложений WindowsDefenderApplicationControl.|
|roleScopeTagIds|Коллекция объектов string|Список тегов области для этого объекта дополнительной политики WindowsDefenderApplicationControl.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|Связанные групповые назначения для этой дополнительной политики WindowsDefenderApplicationControl.|
|deploySummary|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|Сводка развертывания дополнительных политик WindowsDefenderApplicationControl.|
|deviceStatuses|[коллекция windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Список состояния развертывания устройств для этой дополнительной политики WindowsDefenderApplicationControl.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "content": "binary",
  "contentFileName": "String",
  "version": "String",
  "creationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ]
}
```




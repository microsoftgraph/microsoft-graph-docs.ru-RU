---
title: Тип ресурса Виндовсдефендераппликатионконтролсупплементалполици
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 865e866db17e1132aef41671b907072122beb2f8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733135"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicy-resource-type"></a>Тип ресурса Виндовсдефендераппликатионконтролсупплементалполици

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список ВиндовсдефендераппликатионконтролсупплементалполиЦиес](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-list.md)|Коллекция [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|Список свойств и связей объектов [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) .|
|[Получение Виндовсдефендераппликатионконтролсупплементалполици](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-get.md)|[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|Чтение свойств и связей объекта [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) .|
|[Создание Виндовсдефендераппликатионконтролсупплементалполици](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-create.md)|[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|Создание нового объекта [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) .|
|[Удаление Виндовсдефендераппликатионконтролсупплементалполици](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-delete.md)|Нет|Удаляет объект [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md).|
|[Обновление Виндовсдефендераппликатионконтролсупплементалполици](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-update.md)|[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|Обновление свойств объекта [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) .|
|[Действие assign](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ для дополнительной политики Виндовсдефендераппликатионконтрол.|
|displayName|Строка|Отображаемое имя дополнительной политики Виндовсдефендераппликатионконтрол.|
|description|Строка|Описание дополнительной политики Виндовсдефендераппликатионконтрол.|
|содержимое|Binary|Содержимое дополнительной политики Виндовсдефендераппликатионконтрол в формате массива байтов.|
|контентфиленаме|Строка|Имя файла дополнительной политики Виндовсдефендераппликатионконтрол.|
|version|String|Версия дополнительной политики Виндовсдефендераппликатионконтрол.|
|креатиондатетиме|DateTimeOffset|Дата и время отправки дополнительной политики Виндовсдефендераппликатионконтрол.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения дополнительной политики Виндовсдефендераппликатионконтрол.|
|roleScopeTagIds|Коллекция строк|Список тегов областей для данной дополнительной политики Виндовсдефендераппликатионконтрол.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|Связанные назначения группы для этой дополнительной политики Виндовсдефендераппликатионконтрол.|
|деплойсуммари|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|Дополнительные сведения о развертывании дополнительной политики Виндовсдефендераппликатионконтрол.|
|deviceStatuses|Коллекция [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Список состояний развертывания устройств для этой дополнительной политики Виндовсдефендераппликатионконтрол.|

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






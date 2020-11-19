---
title: Тип ресурса Унсуппортедграупполициекстенсион
description: Неподдерживаемое расширение групповой политики.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ca972c300bfd2c4d8da5c6da780f1ef21306f5ff
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298570"
---
# <a name="unsupportedgrouppolicyextension-resource-type"></a>Тип ресурса Унсуппортедграупполициекстенсион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Неподдерживаемое расширение групповой политики.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Унсуппортедграупполициекстенсионс](../api/intune-gpanalyticsservice-unsupportedgrouppolicyextension-list.md)|Коллекция [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)|Список свойств и связей объектов [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) .|
|[Получение Унсуппортедграупполициекстенсион](../api/intune-gpanalyticsservice-unsupportedgrouppolicyextension-get.md)|[unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)|Чтение свойств и связей объекта [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) .|
|[Создание Унсуппортедграупполициекстенсион](../api/intune-gpanalyticsservice-unsupportedgrouppolicyextension-create.md)|[unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)|Создание нового объекта [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) .|
|[Удаление Унсуппортедграупполициекстенсион](../api/intune-gpanalyticsservice-unsupportedgrouppolicyextension-delete.md)|Нет|Удаляет объект [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md).|
|[Обновление Унсуппортедграупполициекстенсион](../api/intune-gpanalyticsservice-unsupportedgrouppolicyextension-update.md)|[unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)|Обновление свойств объекта [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Пока не задокументировано.|
|сеттингскопе|[groupPolicySettingScope](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|Задание области для неподдерживаемого расширения. Возможные значения: `unknown`, `device`, `user`.|
|намеспацеурл|String|URL-адрес пространства имен неподдерживаемого расширения.|
|екстенсионтипе|String|Екстенсионтипе неподдерживаемого расширения.|
|nodeName|String|Имя узла неподдерживаемого расширения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unsupportedGroupPolicyExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unsupportedGroupPolicyExtension",
  "id": "String (identifier)",
  "settingScope": "String",
  "namespaceUrl": "String",
  "extensionType": "String",
  "nodeName": "String"
}
```





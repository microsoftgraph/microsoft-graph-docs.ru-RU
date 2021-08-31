---
title: тип ресурса unsupportedGroupPolicyExtension
description: Расширение групповой политики без поддержки.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 133a6b5605f7a8efe880eb71d3354ba59623152b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58785705"
---
# <a name="unsupportedgrouppolicyextension-resource-type"></a>тип ресурса unsupportedGroupPolicyExtension

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Расширение групповой политики без поддержки.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список неподтвершенныхGroupPolicyExtensions](../api/intune-gpanalyticsservice-unsupportedgrouppolicyextension-list.md)|[коллекция unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)|Список свойств и связей неподтвершенных [объектовGroupPolicyExtension.](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)|
|[Получить неподтвершеннуюGroupPolicyExtension](../api/intune-gpanalyticsservice-unsupportedgrouppolicyextension-get.md)|[unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)|Чтение свойств и связей неподтвершенного [объектаGroupPolicyExtension.](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)|
|[Создание неподтвердимойGroupPolicyExtension](../api/intune-gpanalyticsservice-unsupportedgrouppolicyextension-create.md)|[unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)|Создайте новый [объект UnsupportedGroupPolicyExtension.](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)|
|[Удаление неподтвершеннойGroupPolicyExtension](../api/intune-gpanalyticsservice-unsupportedgrouppolicyextension-delete.md)|Нет|Удаляет [неподтвершеннуюGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md).|
|[Обновление неподтвершеннойGroupPolicyExtension](../api/intune-gpanalyticsservice-unsupportedgrouppolicyextension-update.md)|[unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)|Обновление свойств неподтвершенного [объектаGroupPolicyExtension.](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Пока не задокументировано.|
|settingScope|[groupPolicySettingScope](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|Настройка области неподтверченного расширения. Возможные значения: `unknown`, `device`, `user`.|
|namespaceUrl|Строка|Url-адрес пространства имен неподтверченного расширения.|
|extensionType|Строка|ExtensionType неподтверченного расширения.|
|nodeName|Строка|Имя узла неподтверченного расширения.|

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




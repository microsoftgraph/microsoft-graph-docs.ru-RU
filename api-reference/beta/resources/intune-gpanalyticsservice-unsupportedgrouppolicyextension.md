---
title: тип ресурса unsupportedGroupPolicyExtension
description: Расширение групповой политики без поддержки.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e4c0493854e17204cf9e81231565ccd50d1bf3c2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086143"
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
|id|String|Пока не задокументировано.|
|settingScope|[groupPolicySettingScope](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|Настройка области неподтверченного расширения. Возможные значения: `unknown`, `device`, `user`.|
|namespaceUrl|String|Url-адрес пространства имен неподтверченного расширения.|
|extensionType|String|ExtensionType неподтверченного расширения.|
|nodeName|String|Имя узла неподтверченного расширения.|

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




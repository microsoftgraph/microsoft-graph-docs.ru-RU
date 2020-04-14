---
title: Тип ресурса Таржетедманажедаппконфигуратионполицисетитем
description: Класс, содержащий свойства, которые используются для целевой Полицисетитем конфигурации управляемого приложения.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bc75e0bd3f32bb8a08fe5b8c214909bf9df11da0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463354"
---
# <a name="targetedmanagedappconfigurationpolicysetitem-resource-type"></a>Тип ресурса Таржетедманажедаппконфигуратионполицисетитем

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, которые используются для целевой Полицисетитем конфигурации управляемого приложения.


Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Таржетедманажедаппконфигуратионполицисетитемс](../api/intune-policyset-targetedmanagedappconfigurationpolicysetitem-list.md)|Коллекция [таржетедманажедаппконфигуратионполицисетитем](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md)|Список свойств и связей объектов [таржетедманажедаппконфигуратионполицисетитем](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) .|
|[Получение Таржетедманажедаппконфигуратионполицисетитем](../api/intune-policyset-targetedmanagedappconfigurationpolicysetitem-get.md)|[targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md)|Чтение свойств и связей объекта [таржетедманажедаппконфигуратионполицисетитем](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) .|
|[Создание Таржетедманажедаппконфигуратионполицисетитем](../api/intune-policyset-targetedmanagedappconfigurationpolicysetitem-create.md)|[targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md)|Создание нового объекта [таржетедманажедаппконфигуратионполицисетитем](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) .|
|[Удаление Таржетедманажедаппконфигуратионполицисетитем](../api/intune-policyset-targetedmanagedappconfigurationpolicysetitem-delete.md)|Нет|Удаляет объект [таржетедманажедаппконфигуратионполицисетитем](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md).|
|[Обновление Таржетедманажедаппконфигуратионполицисетитем](../api/intune-policyset-targetedmanagedappconfigurationpolicysetitem-update.md)|[targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md)|Обновление свойств объекта [таржетедманажедаппконфигуратионполицисетитем](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ Мобилеаппполицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|Время создания Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|пайлоадид|String|Пайлоадид Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|itemType|String|Полицисеттипе Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|displayName|Строка|DisplayName объекта Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Состояние Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md). Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Код ошибки (при возникновении ошибки). Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md). Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.|
|гуидеддеплойменттагс|Коллекция String|Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppConfigurationPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfigurationPolicySetItem",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "payloadId": "String",
  "itemType": "String",
  "displayName": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ]
}
```




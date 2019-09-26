---
title: Тип ресурса Иослобапппровисионингконфигуратионполицисетитем
description: Класс, содержащий свойства, используемые для настройки подготовки бизнес-приложений iOS Полицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4bee69b2ae7817bf0419fcaca4bf7b1064f0506b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201266"
---
# <a name="ioslobappprovisioningconfigurationpolicysetitem-resource-type"></a>Тип ресурса Иослобапппровисионингконфигуратионполицисетитем

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для настройки подготовки бизнес-приложений iOS Полицисетитем.


Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Иослобапппровисионингконфигуратионполицисетитемс](../api/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem-list.md)|Коллекция [иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)|Список свойств и связей объектов [иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) .|
|[Получение Иослобапппровисионингконфигуратионполицисетитем](../api/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem-get.md)|[иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)|Чтение свойств и связей объекта [иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) .|
|[Создание Иослобапппровисионингконфигуратионполицисетитем](../api/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem-create.md)|[иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)|Создание нового объекта [иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) .|
|[Удаление Иослобапппровисионингконфигуратионполицисетитем](../api/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem-delete.md)|Нет|Удаляет объект [иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md).|
|[Обновление Иослобапппровисионингконфигуратионполицисетитем](../api/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem-update.md)|[иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)|Обновление свойств объекта [иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ Мобилеаппполицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|Время создания Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|пайлоадид|String.|Пайлоадид Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|itemType|String.|Полицисеттипе Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|displayName|Строка|DisplayName объекта Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|status|[полицисетстатус](../resources/intune-policyset-policysetstatus.md)|Состояние Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md). Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[Коде](../resources/intune-policyset-errorcode.md)|Код ошибки (при возникновении ошибки). Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md). Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.|
|гуидеддеплойменттагс|Коллекция строк|Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosLobAppProvisioningConfigurationPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationPolicySetItem",
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




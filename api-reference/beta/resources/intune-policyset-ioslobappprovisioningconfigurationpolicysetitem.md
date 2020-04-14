---
title: Тип ресурса Иослобапппровисионингконфигуратионполицисетитем
description: Класс, содержащий свойства, используемые для настройки подготовки бизнес-приложений iOS Полицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7b58d4a68f3324f103cd2a792a5b202eb2ea53d4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458405"
---
# <a name="ioslobappprovisioningconfigurationpolicysetitem-resource-type"></a>Тип ресурса Иослобапппровисионингконфигуратионполицисетитем

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для настройки подготовки бизнес-приложений iOS Полицисетитем.


Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Иослобапппровисионингконфигуратионполицисетитемс](../api/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem-list.md)|Коллекция [иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)|Список свойств и связей объектов [иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) .|
|[Получение Иослобапппровисионингконфигуратионполицисетитем](../api/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem-get.md)|[iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)|Чтение свойств и связей объекта [иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) .|
|[Создание Иослобапппровисионингконфигуратионполицисетитем](../api/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem-create.md)|[iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)|Создание нового объекта [иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) .|
|[Удаление Иослобапппровисионингконфигуратионполицисетитем](../api/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem-delete.md)|Нет|Удаляет объект [иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md).|
|[Обновление Иослобапппровисионингконфигуратионполицисетитем](../api/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem-update.md)|[iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)|Обновление свойств объекта [иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) .|

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

## <a name="relationships"></a>Связи
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




---
title: Тип ресурса Девицекомплианцеполициполицисетитем
description: Класс, содержащий свойства, используемые для политики соответствия требованиям устройств Полицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8e280cb35dc5f87fdc970c84632cfbca80f1da90
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259370"
---
# <a name="devicecompliancepolicypolicysetitem-resource-type"></a>Тип ресурса Девицекомплианцеполициполицисетитем

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для политики соответствия требованиям устройств Полицисетитем.


Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицекомплианцеполициполицисетитемс](../api/intune-policyset-devicecompliancepolicypolicysetitem-list.md)|Коллекция [девицекомплианцеполициполицисетитем](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)|Список свойств и связей объектов [девицекомплианцеполициполицисетитем](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) .|
|[Получение Девицекомплианцеполициполицисетитем](../api/intune-policyset-devicecompliancepolicypolicysetitem-get.md)|[deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)|Чтение свойств и связей объекта [девицекомплианцеполициполицисетитем](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) .|
|[Создание Девицекомплианцеполициполицисетитем](../api/intune-policyset-devicecompliancepolicypolicysetitem-create.md)|[deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)|Создание нового объекта [девицекомплианцеполициполицисетитем](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) .|
|[Удаление Девицекомплианцеполициполицисетитем](../api/intune-policyset-devicecompliancepolicypolicysetitem-delete.md)|Нет|Удаляет объект [девицекомплианцеполициполицисетитем](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md).|
|[Обновление Девицекомплианцеполициполицисетитем](../api/intune-policyset-devicecompliancepolicypolicysetitem-update.md)|[deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)|Обновление свойств объекта [девицекомплианцеполициполицисетитем](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ Мобилеаппполицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|Время создания Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|пайлоадид|String|Пайлоадид Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|itemType|String|Полицисеттипе Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|displayName|String|DisplayName объекта Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Состояние Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md). Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Код ошибки (при возникновении ошибки). Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md). Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.|
|гуидеддеплойменттагс|Коллекция строк|Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyPolicySetItem",
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





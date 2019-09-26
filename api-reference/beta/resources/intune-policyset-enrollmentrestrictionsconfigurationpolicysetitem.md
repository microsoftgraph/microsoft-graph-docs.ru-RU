---
title: Тип ресурса Енроллментрестриктионсконфигуратионполицисетитем
description: Класс, содержащий свойства, используемые для ограничения регистрации Полицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e119bb47081316cc7f91cd05aadf6b133efea6d5
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201274"
---
# <a name="enrollmentrestrictionsconfigurationpolicysetitem-resource-type"></a>Тип ресурса Енроллментрестриктионсконфигуратионполицисетитем

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для ограничения регистрации Полицисетитем.


Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Енроллментрестриктионсконфигуратионполицисетитемс](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-list.md)|Коллекция [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)|Список свойств и связей объектов [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) .|
|[Получение Енроллментрестриктионсконфигуратионполицисетитем](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-get.md)|[енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)|Чтение свойств и связей объекта [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) .|
|[Создание Енроллментрестриктионсконфигуратионполицисетитем](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-create.md)|[енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)|Создание нового объекта [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) .|
|[Удаление Енроллментрестриктионсконфигуратионполицисетитем](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-delete.md)|Нет|Удаляет объект [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md).|
|[Обновление Енроллментрестриктионсконфигуратионполицисетитем](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-update.md)|[енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)|Обновление свойств объекта [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) .|

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
|priority|Int32|Приоритет Енроллментрестриктионсконфигуратионполицисетитем.|
|limit|Int32|Ограничения для Енроллментрестриктионсконфигуратионполицисетитем.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem",
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
  ],
  "priority": 1024,
  "limit": 1024
}
```




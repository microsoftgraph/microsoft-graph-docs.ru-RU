---
title: Тип ресурса Енроллментрестриктионсконфигуратионполицисетитем
description: Класс, содержащий свойства, используемые для ограничения регистрации Полицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9377854bb4c543147938ca785f87f539bca59de1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458442"
---
# <a name="enrollmentrestrictionsconfigurationpolicysetitem-resource-type"></a>Тип ресурса Енроллментрестриктионсконфигуратионполицисетитем

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для ограничения регистрации Полицисетитем.


Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Енроллментрестриктионсконфигуратионполицисетитемс](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-list.md)|Коллекция [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)|Список свойств и связей объектов [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) .|
|[Получение Енроллментрестриктионсконфигуратионполицисетитем](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-get.md)|[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)|Чтение свойств и связей объекта [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) .|
|[Создание Енроллментрестриктионсконфигуратионполицисетитем](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-create.md)|[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)|Создание нового объекта [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) .|
|[Удаление Енроллментрестриктионсконфигуратионполицисетитем](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-delete.md)|Нет|Удаляет объект [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md).|
|[Обновление Енроллментрестриктионсконфигуратионполицисетитем](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-update.md)|[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)|Обновление свойств объекта [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) .|

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
|priority|Int32|Приоритет Енроллментрестриктионсконфигуратионполицисетитем.|
|limit|Int32|Ограничения для Енроллментрестриктионсконфигуратионполицисетитем.|

## <a name="relationships"></a>Связи
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




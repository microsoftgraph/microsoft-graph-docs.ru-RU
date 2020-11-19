---
title: Тип ресурса Виндовсаутопилотдеплойментпрофилеполицисетитем
description: Класс, содержащий свойства, используемые для профиля развертывания Windows Полицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 04ba3d6eab82e49bd87f5488fd758e413081d426
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49266286"
---
# <a name="windowsautopilotdeploymentprofilepolicysetitem-resource-type"></a>Тип ресурса Виндовсаутопилотдеплойментпрофилеполицисетитем

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для профиля развертывания Windows Полицисетитем.


Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсаутопилотдеплойментпрофилеполицисетитемс](../api/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem-list.md)|Коллекция [виндовсаутопилотдеплойментпрофилеполицисетитем](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)|Список свойств и связей объектов [виндовсаутопилотдеплойментпрофилеполицисетитем](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) .|
|[Получение Виндовсаутопилотдеплойментпрофилеполицисетитем](../api/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem-get.md)|[windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)|Чтение свойств и связей объекта [виндовсаутопилотдеплойментпрофилеполицисетитем](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) .|
|[Создание Виндовсаутопилотдеплойментпрофилеполицисетитем](../api/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem-create.md)|[windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)|Создание нового объекта [виндовсаутопилотдеплойментпрофилеполицисетитем](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) .|
|[Удаление Виндовсаутопилотдеплойментпрофилеполицисетитем](../api/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem-delete.md)|Нет|Удаляет объект [виндовсаутопилотдеплойментпрофилеполицисетитем](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md).|
|[Обновление Виндовсаутопилотдеплойментпрофилеполицисетитем](../api/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem-update.md)|[windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)|Обновление свойств объекта [виндовсаутопилотдеплойментпрофилеполицисетитем](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) .|

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
  "@odata.type": "microsoft.graph.windowsAutopilotDeploymentProfilePolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfilePolicySetItem",
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





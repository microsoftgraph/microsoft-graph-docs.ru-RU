---
title: тип ресурса customExtensionHandler
description: Определяет, когда необходимо выполнить расширение рабочего процесса пакета пользовательского доступа.
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 59873faa46acb6f258ca6308da2b9d29e323bf65
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339047"
---
# <a name="customextensionhandler-resource-type"></a>тип ресурса customExtensionHandler

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет, когда необходимо выполнить расширение рабочего процесса пакета [пользовательского доступа](customaccesspackageworkflowextension.md).

Наследуется [от сущности](entity.md).

## <a name="methods"></a>Методы
Нет.

> [!NOTE]
>
> 1. Чтобы ознакомиться с объектами customExtensionHandler в политике, `?$expand=customExtensionHandlers` в приложении к [запросу GET accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) . Например, `GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/4540a08f-8ab5-43f6-a923-015275799197?$expand=customExtensionHandlers`. Дополнительные сведения см [. в примере 2. Извлечение пользовательских обработчиков расширения для политики](../api/accesspackageassignmentpolicy-get.md#example-2-retrieve-the-custom-extension-handlers-for-a-policy).
>
> 2. Чтобы удалить **объекты customExtensionHandlers** из политики, позвоните в update [accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md) и укажите свойство customExtensionHandlers в качестве пустой коллекции. Дополнительные сведения см [. в примере 2. Удалите настраиваемыеExtensionHandlers из политики](../api/accesspackageassignmentpolicy-update.md#example-2-remove-the-customextensionhandlers-from-a-policy).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка| Идентификатор сцены. Наследуется [от сущности](../resources/entity.md).|
|этап|accessPackageCustomExtensionStage|Указывает этап рабочего процесса запроса запроса на назначение пакета доступа при запуске настраиваемого расширения пакета доступа. Возможные значения: `assignmentRequestCreated`, `assignmentRequestApproved`, `assignmentRequestGranted`, `assignmentRequestRemoved`, `assignmentFourteenDaysBeforeExpiration`, `assignmentOneDayBeforeExpiration`, `unknownFutureValue`. |

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|customExtension|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|Указывает, какое пользовательское расширение рабочего процесса будет выполнено на данном этапе. Допускается значение null. Поддерживает `$expand`.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.customExtensionHandler",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customExtensionHandler",
  "id": "String (identifier)",
  "stage": "String"
}
```


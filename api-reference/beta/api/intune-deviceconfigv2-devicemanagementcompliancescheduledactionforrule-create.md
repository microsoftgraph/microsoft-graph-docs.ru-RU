---
title: Создание deviceManagementComplianceScheduledActionForRule
description: Создание нового объекта deviceManagementComplianceScheduledActionForRule.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c4c58ad66de0d6d92d95ff34db487056a6d016f4
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695654"
---
# <a name="create-devicemanagementcompliancescheduledactionforrule"></a>Создание deviceManagementComplianceScheduledActionForRule

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта deviceManagementComplianceScheduledActionForRule.](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/compliancePolicies/{deviceManagementCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта deviceManagementComplianceScheduledActionForRule.

В следующей таблице показаны свойства, необходимые при создании устройстваManagementComplianceScheduledActionForRule.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ этого параметра в политике, содержа которой он содержится. Автоматически созданный.|
|ruleName|String|Имя правила, к которому применяется это запланированное действие.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа и `201 Created` [объект deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/compliancePolicies/{deviceManagementCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementComplianceScheduledActionForRule",
  "id": "4d62ccbd-ccbd-4d62-bdcc-624dbdcc624d",
  "ruleName": "Rule Name value"
}
```




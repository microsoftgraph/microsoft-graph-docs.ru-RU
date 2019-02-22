---
title: Действие assign
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4cf7440dd856731a0079ce7781b4c9c05d932d9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151655"
---
# <a name="assign-action"></a>Действие назначения

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано.

## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тело запроса добавьте параметры в формате JSON.

В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.

|Свойство|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Н/Д|



## <a name="response"></a>Отклик
При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign

Content-type: application/json
Content-length: 350

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





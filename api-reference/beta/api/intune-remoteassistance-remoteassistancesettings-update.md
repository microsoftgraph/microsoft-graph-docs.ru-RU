---
title: Обновление remoteAssistanceSettings
description: Обновление свойств объекта remoteAssistanceSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e3d81fbdbab253866de523d6d0c4083b29dc204d
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61343688"
---
# <a name="update-remoteassistancesettings"></a>Обновление remoteAssistanceSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [remoteAssistanceSettings.](../resources/intune-remoteassistance-remoteassistancesettings.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistanceSettings
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта [remoteAssistanceSettings.](../resources/intune-remoteassistance-remoteassistancesettings.md)

В следующей таблице показаны свойства, необходимые при создании [remoteAssistanceSettings.](../resources/intune-remoteassistance-remoteassistancesettings.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор параметров удаленной помощи|
|remoteAssistanceState|[remoteAssistanceState](../resources/intune-remoteassistance-remoteassistancestate.md)|Текущее состояние удаленной помощи для учетной записи. Возможные значения: отключено, включено. Этот параметр настраивается администратором. Параметры удаленной помощи, которые еще не настроены администратором, отключены. Возвращается по умолчанию. Возможные значения: `disabled`, `enabled`.|
|allowSessionsToUnenrolledDevices|Boolean| Указывает, разрешены ли сеансы для незавершенных устройств для учетной записи. Этот параметр настраивается администратором. Значение по умолчанию является ложным.|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект remoteAssistanceSettings](../resources/intune-remoteassistance-remoteassistancesettings.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteAssistanceSettings
Content-type: application/json
Content-length: 150

{
  "@odata.type": "#microsoft.graph.remoteAssistanceSettings",
  "remoteAssistanceState": "enabled",
  "allowSessionsToUnenrolledDevices": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 199

{
  "@odata.type": "#microsoft.graph.remoteAssistanceSettings",
  "id": "cfef360e-360e-cfef-0e36-efcf0e36efcf",
  "remoteAssistanceState": "enabled",
  "allowSessionsToUnenrolledDevices": true
}
```





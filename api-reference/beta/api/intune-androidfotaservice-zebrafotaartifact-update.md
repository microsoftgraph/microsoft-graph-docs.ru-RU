---
title: Обновление zebraFotaArtifact
description: Обновление свойств объекта zebraFotaArtifact.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0c3af33735b3d683db14b5d2137734abaf0354eb
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213511"
---
# <a name="update-zebrafotaartifact"></a>Обновление zebraFotaArtifact

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/zebraFotaArtifacts/{zebraFotaArtifactId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md) в формате JSON.

В следующей таблице показаны свойства, необходимые при создании [объекта zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор ZebraFotaArtifact.|
|deviceModel|String|Модель артефакта устройства.|
|osVersion|String|Версия ОС артефакта.|
|patchVersion|Строка|Версия исправления артефакта.|
|boardSupportPackageVersion|Строка|Версия пакета поддержки Board.|
|releaseNotesUrl|Строка|URL-адрес заметок о выпуске артефакта.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код `200 OK` отклика и обновленный объект [zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/zebraFotaArtifacts/{zebraFotaArtifactId}
Content-type: application/json
Content-length: 311

{
  "@odata.type": "#microsoft.graph.zebraFotaArtifact",
  "deviceModel": "Device Model value",
  "osVersion": "Os Version value",
  "patchVersion": "Patch Version value",
  "boardSupportPackageVersion": "Board Support Package Version value",
  "releaseNotesUrl": "https://example.com/releaseNotesUrl/"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 360

{
  "@odata.type": "#microsoft.graph.zebraFotaArtifact",
  "id": "37305f61-5f61-3730-615f-3037615f3037",
  "deviceModel": "Device Model value",
  "osVersion": "Os Version value",
  "patchVersion": "Patch Version value",
  "boardSupportPackageVersion": "Board Support Package Version value",
  "releaseNotesUrl": "https://example.com/releaseNotesUrl/"
}
```





---
title: Создание Виндовсдефендераппликатионконтролсупплементалполици
description: Создание нового объекта Виндовсдефендераппликатионконтролсупплементалполици.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 129520508a671c10fb6719ea072a167cd5fe17a7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692725"
---
# <a name="create-windowsdefenderapplicationcontrolsupplementalpolicy"></a>Создание Виндовсдефендераппликатионконтролсупплементалполици

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта Виндовсдефендераппликатионконтролсупплементалполици в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Виндовсдефендераппликатионконтролсупплементалполици.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ для дополнительной политики Виндовсдефендераппликатионконтрол.|
|displayName|Строка|Отображаемое имя дополнительной политики Виндовсдефендераппликатионконтрол.|
|description|Строка|Описание дополнительной политики Виндовсдефендераппликатионконтрол.|
|содержимое|Binary|Содержимое дополнительной политики Виндовсдефендераппликатионконтрол в формате массива байтов.|
|контентфиленаме|Строка|Имя файла дополнительной политики Виндовсдефендераппликатионконтрол.|
|version|String|Версия дополнительной политики Виндовсдефендераппликатионконтрол.|
|креатиондатетиме|DateTimeOffset|Дата и время отправки дополнительной политики Виндовсдефендераппликатионконтрол.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения дополнительной политики Виндовсдефендераппликатионконтрол.|
|roleScopeTagIds|Коллекция строк|Список тегов областей для данной дополнительной политики Виндовсдефендераппликатионконтрол.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "content": "Y29udGVudA==",
  "contentFileName": "Content File Name value",
  "version": "Version value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 517

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "id": "83d0c39e-c39e-83d0-9ec3-d0839ec3d083",
  "displayName": "Display Name value",
  "description": "Description value",
  "content": "Y29udGVudA==",
  "contentFileName": "Content File Name value",
  "version": "Version value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```






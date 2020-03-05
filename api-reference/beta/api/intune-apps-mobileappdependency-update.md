---
title: Обновление Мобилеаппдепенденци
description: Обновление свойств объекта Мобилеаппдепенденци.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1179187b5071530ba76ffb293379714550cd96aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445066"
---
# <a name="update-mobileappdependency"></a>Обновление Мобилеаппдепенденци

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) .

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
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор сущности отношения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)|
|targetId|String|Идентификатор приложения целевого дочернего мобильного приложения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)|
|таржетдисплайнаме|String|Отображаемое имя целевого дочернего мобильного приложения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)|
|депенденцитипе|[mobileAppDependencyType](../resources/intune-apps-mobileappdependencytype.md)|Тип отношения зависимости между родительским и дочерним приложениями. Возможные значения: `detect`, `autoInstall`.|
|депендентаппкаунт|Int32|Общее количество зависимостей для дочернего приложения.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```






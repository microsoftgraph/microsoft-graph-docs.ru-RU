---
title: Создание неподтвердимойGroupPolicyExtension
description: Создайте новый объект UnsupportedGroupPolicyExtension.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 98fd00744ae068f55319321cbe853af9cce3582f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020604"
---
# <a name="create-unsupportedgrouppolicyextension"></a>Создание неподтвердимойGroupPolicyExtension

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте новый [объект UnsupportedGroupPolicyExtension.](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для неподдерживаемого объектаGroupPolicyExtension.

В следующей таблице показаны свойства, необходимые при создании неподтвершеннойGroupPolicyExtension.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Пока не задокументировано.|
|settingScope|[groupPolicySettingScope](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|Настройка области неподтверченного расширения. Возможные значения: `unknown`, `device`, `user`.|
|namespaceUrl|String|Url-адрес пространства имен неподтверченного расширения.|
|extensionType|String|ExtensionType неподтверченного расширения.|
|nodeName|String|Имя узла неподтверченного расширения.|



## <a name="response"></a>Ответ
В случае успешной работы этот метод возвращает код ответа и неподтвердимый `201 Created` [объектGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.unsupportedGroupPolicyExtension",
  "settingScope": "device",
  "namespaceUrl": "https://example.com/namespaceUrl/",
  "extensionType": "Extension Type value",
  "nodeName": "Node Name value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.unsupportedGroupPolicyExtension",
  "id": "e59ecce2-cce2-e59e-e2cc-9ee5e2cc9ee5",
  "settingScope": "device",
  "namespaceUrl": "https://example.com/namespaceUrl/",
  "extensionType": "Extension Type value",
  "nodeName": "Node Name value"
}
```




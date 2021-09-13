---
title: Update groupPolicyPresentationListBox
description: Обновление свойств объекта groupPolicyPresentationListBox.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5477edea5240bb40de2c0659fb5710b509b4af4b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59112316"
---
# <a name="update-grouppolicypresentationlistbox"></a>Update groupPolicyPresentationListBox

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [groupPolicyPresentationListBox.](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта groupPolicyPresentationListBox.](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)

В следующей таблице показаны свойства, необходимые при создании [groupPolicyPresentationListBox.](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|подпись|String|Локализованная текстовая метка для любого объекта презентации. По умолчанию это значение пусто. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Ключ объекта. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|explicitValue|Логическое|Если этот параметр указан верно, пользователь должен указать значение подкайки реестра и имя подкайки реестра. В поле списка показаны два столбца: один для имени и один для данных. Значение по умолчанию  false.|
|valuePrefix|String|Пока не задокументировано.|



## <a name="response"></a>Ответ
В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [GroupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "explicitValue": true,
  "valuePrefix": "Value Prefix value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "id": "2e074c87-4c87-2e07-874c-072e874c072e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "explicitValue": true,
  "valuePrefix": "Value Prefix value"
}
```




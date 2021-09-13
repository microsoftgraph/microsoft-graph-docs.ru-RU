---
title: Создание groupPolicyPresentationLongDecimalTextBox
description: Создайте новый объект groupPolicyPresentationLongDecimalTextBox.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc451eff0d01a8304466f4383ba238a416469d0c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59121594"
---
# <a name="create-grouppolicypresentationlongdecimaltextbox"></a>Создание groupPolicyPresentationLongDecimalTextBox

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте новый [объект groupPolicyPresentationLongDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)

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
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса предопределите представление JSON для объекта GroupPolicyPresentationLongDecimalTextBox.

В следующей таблице показаны свойства, необходимые при создании группыPolicyPresentationLongDecimalTextBox.

|Свойство|Тип|Описание|
|:---|:---|:---|
|подпись|String|Локализованная текстовая метка для любого объекта презентации. По умолчанию это значение пусто. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Ключ объекта. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|defaultValue|Int64|Неподписаный полный ящик, который указывает начальное значение десятичной текстовой коробки. Значение по умолчанию равно 1.|
|spin|Логическое|Если верно, создайте управление спином; в противном случае создайте текстовое поле для числовой записи. Значение по умолчанию: true.|
|spinStep|Int64|Неподписавая часть, указывляемая на приращение изменений для управления спином. Значение по умолчанию равно 1.|
|обязательно|Логическое|Требование ввести значение в поле параметра. Значение по умолчанию  false.|
|minValue|Int64|Неподписаный длинный, который указывает минимально допустимые значения. Значение по умолчанию равно 0.|
|maxValue|Int64|Неподписаное длинное значение, которое указывает максимально допустимые значения. Значение по умолчанию — 9999.|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 225

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
  "label": "Label value",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 338

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
  "label": "Label value",
  "id": "754d8495-8495-754d-9584-4d7595844d75",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```




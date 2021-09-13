---
title: тип ресурса encryptionReportPolicyDetails
description: Сведения о политике для отчета о шифровании
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ad1ea4b2002f4689fdfe905f8de4c59e29e7f30f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59101473"
---
# <a name="encryptionreportpolicydetails-resource-type"></a>тип ресурса encryptionReportPolicyDetails

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения о политике для отчета о шифровании

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|policyId|String|Код политики для отчета о шифровании|
|policyName|String|Имя политики для отчета о шифровании|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.encryptionReportPolicyDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.encryptionReportPolicyDetails",
  "policyId": "String",
  "policyName": "String"
}
```




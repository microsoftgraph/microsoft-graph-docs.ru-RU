---
title: тип ресурса encryptionReportPolicyDetails
description: Сведения о политике для отчета о шифровании
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 84a5f10542db3f2677cda68923eebf1bc2fb4008bfb0ee6a2669fd8be33f6951
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54241968"
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
|policyName|Строка|Имя политики для отчета о шифровании|

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





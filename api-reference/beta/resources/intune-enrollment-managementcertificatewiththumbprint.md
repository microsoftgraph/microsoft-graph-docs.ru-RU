---
title: Тип ресурса Манажементцертификатевиссумбпринт
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f497780f9ccd21ea608a8c7e56e6926d79263e24
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963480"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a>Тип ресурса Манажементцертификатевиссумбпринт

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|отпечаток|String|Отпечаток сертификата управления|
|certificate|String|Сертификат управления Base 64 с шифрованием|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementCertificateWithThumbprint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCertificateWithThumbprint",
  "thumbprint": "String",
  "certificate": "String"
}
```






---
title: Тип ресурса fileEncryptionInfo
description: Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7c020aa549e9e9a7c2520db6893d0cc60f65b8a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988284"
---
# <a name="fileencryptioninfo-resource-type"></a>Тип ресурса fileEncryptionInfo

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|encryptionKey|Binary|Ключ, используемый для шифрования содержимого файла.|
|initializationVector|Binary|Вектор инициализации, используемый для алгоритма шифрования.|
|mac|Binary|Хэш зашифрованного содержимого файла + IV (хэш содержимого).|
|macKey|Binary|Ключ для получения свойства mac.|
|profileIdentifier|String|Идентификатор профиля.|
|fileDigest|Binary|Дайджест файла до шифрования.|
|fileDigestAlgorithm|String|Алгоритм дайджеста файла.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileEncryptionInfo",
  "encryptionKey": "binary",
  "initializationVector": "binary",
  "mac": "binary",
  "macKey": "binary",
  "profileIdentifier": "String",
  "fileDigest": "binary",
  "fileDigestAlgorithm": "String"
}
```










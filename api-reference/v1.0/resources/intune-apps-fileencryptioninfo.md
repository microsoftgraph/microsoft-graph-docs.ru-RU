---
title: Тип ресурса fileEncryptionInfo
description: Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7faee233b15a4303abe39b4b45a8bc1f0aa19d3c37d3c0c8045098be11228965
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152630"
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





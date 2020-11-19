---
title: Тип ресурса fileEncryptionInfo
description: Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e5bb90354172fab1f691a49b2488871109df3532
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49274273"
---
# <a name="fileencryptioninfo-resource-type"></a>Тип ресурса fileEncryptionInfo

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

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





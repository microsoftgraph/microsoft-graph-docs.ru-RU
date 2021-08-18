---
title: Тип ресурса fileEncryptionInfo
description: Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 925b8ec1d64461b6a02b131bf775c9c60464cbdd106def46c96a36ba15cf2d09
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54153309"
---
# <a name="fileencryptioninfo-resource-type"></a>Тип ресурса fileEncryptionInfo

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

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





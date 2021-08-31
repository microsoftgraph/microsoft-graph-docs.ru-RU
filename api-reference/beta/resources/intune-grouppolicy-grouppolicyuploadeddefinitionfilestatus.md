---
title: groupPolicyUploadedDefinitionFileStatus enum type
description: Тип групповой политики, загруженный в файл определения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 49a0bde51eb726b72c1978d5323f9c6699895d80
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58784781"
---
# <a name="grouppolicyuploadeddefinitionfilestatus-enum-type"></a>groupPolicyUploadedDefinitionFileStatus enum type

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип групповой политики, загруженный в файл определения.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|0|Group Policy uploaded definition file invalid upload status.|
|uploadInProgress|1|Group Policy uploaded definition file upload in progress.|
|доступен|2|Файл определения, загруженный групповой политикой, доступен.|
|назначено|3|Файл определения групповой политики, загруженный в политику.|
|removalInProgress|4 |Group Policy uploaded definition file removal in progress.|
|uploadFailed|5 |Отправка файла определения групповой политики не удалась.|
|removalFailed|6 |Удаление файлов определения групповой политики не удалось.|




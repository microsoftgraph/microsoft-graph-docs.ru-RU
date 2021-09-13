---
title: groupPolicyUploadedDefinitionFileStatus enum type
description: Тип групповой политики, загруженный в файл определения.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 765300d2af833a2dfaa8e6b42aac47281da01d1f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030188"
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




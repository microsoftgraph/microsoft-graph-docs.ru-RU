---
title: тип enum applicationGuardBlockClipboardSharingType
description: Возможные значения для приложенияGuardBlockClipboardSharingType
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 52ce5dbdbbe2c13c3d07b6797770cb089cf8e7f8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59106331"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a>тип enum applicationGuardBlockClipboardSharingType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для приложенияGuardBlockClipboardSharingType

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Not Configured|
|blockBoth|1|Блокировка буфера обмена данными как от хоста до контейнера, так и от контейнера к хосту|
|blockHostToContainer|2|Блокировка буфера обмена данными с хост-контейнера|
|blockContainerToHost|3|Блокировка буфера обмена данными из контейнера в хост|
|blockNone|4 |Блокировка буфера обмена данными ни от хоста до контейнера, ни от контейнера к хосту|




---
title: тип enum applicationGuardBlockClipboardSharingType
description: Возможные значения для приложенияGuardBlockClipboardSharingType
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 879d61352702e0eb7a6b3b77b462ed9c24e0fd7d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58805761"
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




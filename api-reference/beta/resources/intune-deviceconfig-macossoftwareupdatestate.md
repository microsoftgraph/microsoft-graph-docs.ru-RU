---
title: тип enum macOSSoftwareUpdateState
description: Состояние обновления программного обеспечения MacOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b5082a4c0150aff002fbe29c09ea35cc337f50207b22d82c615360c9e28ea122
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54127112"
---
# <a name="macossoftwareupdatestate-enum-type"></a>тип enum macOSSoftwareUpdateState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние обновления программного обеспечения MacOS

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|success|0|Успешно установлено обновление программного обеспечения|
|загрузка|1000|Загружается обновление программного обеспечения|
|загружено|1001|Скачали обновление программного обеспечения|
|установка|1002|Устанавливается обновление программного обеспечения|
|праздный|1003|В этом обновлении программного обеспечения не принимаются меры|
|доступен|1004|Обновление программного обеспечения доступно на устройстве|
|scheduled|1005|Обновление программного обеспечения запланировано на устройстве|
|downloadFailed|2000|Не удалось скачать обновление программного обеспечения|
|downloadInsufficientSpace|2001|Для скачивания обновления не хватает места|
|downloadInsufficientPower|2002|Не хватает мощности для скачивания обновления|
|downloadInsufficientNetwork|2003|Не хватает емкости сети для скачивания обновления|
|installInsufficientSpace|2004|Для установки обновления недостаточно места|
|installInsufficientPower|2005|Не хватает мощности для установки обновления|
|installFailed|2006|Установка не удалось по неустановленной причине|
|commandFailed|2007|Команда обновления расписания не справилась с работой по неустановленной причине|





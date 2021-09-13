---
title: тип enum macOSSoftwareUpdateState
description: Состояние обновления программного обеспечения MacOS
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3459390263c0494a9c67e83a9f1cb4579db283e2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054494"
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




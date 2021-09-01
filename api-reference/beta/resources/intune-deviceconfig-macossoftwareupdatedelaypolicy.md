---
title: тип enum macOSSoftwareUpdateDelayPolicy
description: Пометить переумен, чтобы определить, откладывать ли обновление программного обеспечения для macOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 16204557d18024d40336b0f73a401141bf48c01a
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58791524"
---
# <a name="macossoftwareupdatedelaypolicy-enum-type"></a>тип enum macOSSoftwareUpdateDelayPolicy

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пометить переумен, чтобы определить, откладывать ли обновление программного обеспечения для macOS.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|0|Задержки обновления программного обеспечения не будут применяться.|
|delayOSUpdateVisibility|1|Принудительное затягивание обновлений программного обеспечения ОС.|
|delayAppUpdateVisibility|2|Задержки усилий для обновлений программного обеспечения приложений.|
|unknownFutureValue|4 |Член Sentinel для случаев, когда клиент не может обрабатывать новые значения в переуме.|
|delayMajorOsUpdateVisibility|8 |Форс-мажорные задержки для основных обновлений программного обеспечения ОС.|




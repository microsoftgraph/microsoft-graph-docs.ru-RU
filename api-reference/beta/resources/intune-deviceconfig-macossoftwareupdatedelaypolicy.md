---
title: тип enum macOSSoftwareUpdateDelayPolicy
description: Пометить переумен, чтобы определить, откладывать ли обновление программного обеспечения для macOS.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 18ce0f39150b4b551b33f7c13dfc96817237617b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054508"
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




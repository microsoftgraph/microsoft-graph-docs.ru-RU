---
title: тип enum defenderPotentiallyUnwantedAppAction
description: Действия защитника по обнаружению потенциально нежелательного приложения (PUA).
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ba0d7de1c865f93edf9341288681aeff2137b632
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59101669"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>тип enum defenderPotentiallyUnwantedAppAction

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Действия защитника по обнаружению потенциально нежелательного приложения (PUA).

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|deviceDefault|0|Защита PUA отключена. Defender не будет защищаться от потенциально нежелательных приложений.|
|block|1|Защита PUA находится в ок. Обнаруженные элементы заблокированы. Они будут показываться в истории вместе с другими угрозами.|
|аудит|2|Режим аудита. Defender обнаруживает потенциально нежелательные приложения, но не принимает никаких действий. Вы можете просмотреть сведения о приложениях, которые защитник принял бы против, ища события, созданные Defender в обозревателе событий.|




---
title: тип enum defenderPotentiallyUnwantedAppAction
description: Действия защитника по обнаружению потенциально нежелательного приложения (PUA).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1ef21f26b259676e774ff009eb8432d4384129fd5977bddf23daf47760742a03
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54142066"
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
|block|1 |Защита PUA находится в ок. Обнаруженные элементы заблокированы. Они будут показываться в истории вместе с другими угрозами.|
|аудит|2|Режим аудита. Defender обнаруживает потенциально нежелательные приложения, но не принимает никаких действий. Вы можете просмотреть сведения о приложениях, которые защитник принял бы против, ища события, созданные Defender в обозревателе событий.|





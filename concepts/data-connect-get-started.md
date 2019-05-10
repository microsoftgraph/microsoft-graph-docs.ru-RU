---
title: Начало работы с подключением к данным Microsoft Graph
description: 'Прежде чем использовать подключение к данным Microsoft Graph, администратору Office 365 необходимо выполнить два действия, которые включают возможность управления перемещением данных для администраторов через Privileged Access Management (PAM). '
author: ajacks-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 8372653d8904ba247975a649e6709b2206a4d6d3
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33599788"
---
# <a name="get-started-with-microsoft-graph-data-connect"></a>Начало работы с подключением к данным Microsoft Graph

Прежде чем использовать подключение к данным Microsoft Graph, администратору Office 365 необходимо выполнить два действия, которые включают возможность управления перемещением данных для администраторов через Privileged Access Management (PAM). 

1. Дайте согласие на участие в подключении данных Microsoft Graph через портал администрирования Microsoft 365 на странице **Службы и надстройки**. Это позволит Microsoft Azure осуществлять запросы на перемещение данных (вы сохраните полный контроль над данными, но разрешите ресурсам Azure доступ к ним). Данные не будут передаваться, пока не будет утвержден определенный конвейер.
2. Настройте утверждающую группу в подписке Office 365. Убедитесь, что утверждающая группа не пустая. Только пользователи в группе могут утверждать запросы на перемещение данных.

## <a name="next-steps"></a>Дальнейшие действия

Поздравляем! Теперь вы готовы к созданию интеллектуальных приложений с помощью инструментария Azure. Чтобы узнать подробные пошаговые инструкции, см. [учебный модуль по подключению данных в Microsoft Graph](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md). Дополнительные сведения о возможностях, предоставляемых подключением к данным Microsoft Graph, см. в статьях о [наборах данных, регионах и приемниках](/concepts/data-connect-datasets.md) и [выборе и фильтрации пользователей](/concepts/data-connect-filtering.md), поддерживаемых подключением к данным.

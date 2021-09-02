---
title: тип переименовки remoteAssistanceOnboardingStatus
description: Текущее состояние соединиттеля TeamViewer
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e89f44ce6df8aaae34e8cab6e5332178d8b6eed2
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58804486"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a>тип переименовки remoteAssistanceOnboardingStatus

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Текущее состояние соединиттеля TeamViewer

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notOnboarded|0|Состояние, сообщаемое при отсутствие активного соединитетеля TeamViewer, настроенного или активного|
|onboarding|1|Состояние, сообщалось, когда система инициировала подключение TeamViewer, но служба еще не завершила подтверждение соединитетеля|
|onboarded|2|Состояние, о чем сообщалось, когда система успешно обменивалась сведениями о учетных записях с TeamViewer и теперь может инициировать сеансы удаленной помощи с клиентами|




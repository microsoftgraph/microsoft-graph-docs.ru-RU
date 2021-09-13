---
title: тип переименовки remoteAssistanceOnboardingStatus
description: Текущее состояние соединиттеля TeamViewer
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ea059025920da62824d816062fe60c03d6b5938d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039485"
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




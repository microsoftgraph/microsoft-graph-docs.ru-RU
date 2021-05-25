---
title: Наборы данных, регионы и приемники, поддерживаемые подключением к данным Microsoft Graph
description: Описаны поддерживаемые наборы данных и типы конечных хранилищ, которые можно использовать с подключением к данным Microsoft Graph.
author: fercobo-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 949f48feec3c0120faf52d992b25cf7438dda577
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629373"
---
# <a name="datasets-regions-and-sinks-that-microsoft-graph-data-connect-supports"></a>Наборы данных, регионы и приемники, поддерживаемые подключением к данным Microsoft Graph

Подключение к данным Microsoft Graph поддерживает разные наборы данных, регионы данных и места хранения в Microsoft Azure. В этой статье описаны поддерживаемые наборы данных и способы доступа к схемам наборов данных, поддерживаемые регионы Microsoft 365 и Microsoft Azure, а также места хранения, используемые подключением к данным с помощью фабрики данных Azure.

## <a name="datasets"></a>Наборы данных

В настоящее время подключение к данным поддерживает следующие наборы данных. Чтобы просмотреть схемы для каждого набора данных, создайте новый набор данных в фабрике данных Azure и используйте для просмотра вкладку "Схема".

<!-- Fernando's note: Some samples are pending, but Nik will update by 5/20 in the GitHub repo. -->
| Имя набора данных                       | Описание                                                                        | Пример |
| ---------------------------------- | ---------------------------------------------------------------------------------- | ------ |
| BasicDataSet_v0.CalendarView_v0    | Содержит события из представления календаря.                                        | [CalendarView_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.CalendarView_v0.json) |
| BasicDataSet_v0.Contact_v0         | Содержит доступные сведения из адресной книги каждого пользователя.                  | Ожидается в ближайшее время!       |
| BasicDataSet_v0.Contact_v1         | Содержит контактные данные из адресной книги каждого пользователя.                        | [Contact_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Contact_v1.json)       |
| BasicDataSet_v0.DirectReport_v0    | Содержит сведения о сотрудниках, находящихся в непосредственном подчинении каждого пользователя.   | [DirectReport_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.DirectReport_v0.json)       |
| BasicDataSet_v0.Event_v0           | Содержит сведения из событий календаря пользователя.                            | Ожидается в ближайшее время!       |
| BasicDataSet_v0.Event_v1           | Содержит события из календаря каждого пользователя.                                       | [Event_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Event_v1.json)       |
| BasicDataSet_v0.MailboxSettings_v0 | Содержит параметры почтового ящика каждого пользователя.                                        | [MailboxSetting_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.MailboxSettings_v0.json)       |
| BasicDataSet_v0.MailFolder_v0      | Содержит папки почты из почтового ящика каждого пользователя.                                | [MailFolder_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.MailFolder_v0.json)       |
| BasicDataSet_v0.Manager_v0         | Содержит сведения о пользователе для руководителя каждого пользователя.                            | [Manager_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Manager_v0.json)       |
| BasicDataSet_v0.Message_v0         | Содержит сообщения из почтового ящика пользователя.                                       | Ожидается в ближайшее время!       |
| BasicDataSet_v0.Message_v1         | Содержит сообщение из почтового ящика каждого пользователя.                                       | [Message_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Message_v1.json)       |
| BasicDataSet_v0.SentItem_v0        | Содержит сообщения, отправленные из почтового ящика каждого пользователя.                               | Ожидается в ближайшее время!       |
| BasicDataSet_v0.SentItem_v1        | Содержит сообщение, отправленное из почтового ящика каждого пользователя.                                | [SentItem_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.SentItem_v1.json)       |
| BasicDataSet_v0.User_v0            | Содержит сведения о пользователе (DisplayName, UserPrincipalName и другую информацию). | Ожидается в ближайшее время!       |
| BasicDataSet_v0.User_v1            | Содержит сведения о пользователе.                                                         | [User_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.User_v1.json)       |

## <a name="regions"></a>Регионы

Подключение к данным поддерживает извлечение данных из множества разных регионов Microsoft 365. Чтобы успешно перенести данные из центра обработки данных Microsoft 365 в свое хранилище Microsoft Azure, экземпляр фабрики данных Azure и место хранения Azure должны быть сопоставлены с поддерживаемым регионом для расположения данных Microsoft 365. В следующей таблице указаны поддерживаемые регионы Microsoft 365 и соответствующие регионы Azure, необходимые для перемещения данных.

| Регион Office      | Регион Azure                                                                                                                                                               |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Азиатско-Тихоокеанский регион**   | <ul><li>Восточная Азия</li><li>Юго-Восточная Азия</li></ul>                                                                                                                         |
| **Австралия**      | <ul><li>Восток Австралии</li><li>Юго-восток Австралии</li></ul>                                                                                                               |
| **Европа**         | <ul><li>Северная Европа</li><li>Западная Европа</li></ul>                                                                                                                         |
| **Северная Америка**  | <ul><li>Центральная часть США</li><li>Восточная часть США</li><li>Восточная часть США 2</li><li>Центрально-северная часть США</li><li>Центрально-южная часть США</li><li>Центрально-западная часть США</li><li>Западная часть США</li><li>Западная часть США 2</li></ul> |
| **Соединенное Королевство** | <ul><li>Южная часть Соединенного Королевства</li><li>Западная часть Соединенного Королевства</li></ul>                                                                                                                                 |

## <a name="sinks"></a>Приемники

Приемники — это выходное расположение, используемое фабрикой данных для размещения данных в хранилище Azure. Подключение к данным поддерживает следующие типы приемных хранилищ:

- [Azure Data Lake Storage 1-го поколения](https://docs.microsoft.com/azure/data-lake-store/data-lake-store-overview)
- [Azure Data Lake Storage 2-го поколения](/azure/storage/blobs/data-lake-storage-introduction)
- [Azure Storage Blob](/azure/storage/blobs/storage-blobs-overview)

К приемникам применяются следующие характеристики:

- Формат выходных файлов: строки JSON. Выходной формат является фиксированным, и его изменение не поддерживается. Однако вы можете использовать фабрику данных Azure для копирования результата конвейера подключения к данным в другой механизм хранения (например, в базу данных Azure SQL).
- Проверка подлинности субъекта-службы является единственным поддерживаемым механизмом проверки подлинности для всех типов приемников при выполнении копирования с использованием Microsoft 365 в качестве источника.
- При использовании хранилища BLOB-объектов Azure в качестве приемника нужно убедиться, что у вашего приложения есть доступ участника данных хранилища BLOB-объектов к расположению хранилища BLOB-объектов Azure.

## <a name="see-also"></a>См. также

- [Соединитель фабрики данных Azure для данных Microsoft 365](https://docs.microsoft.com/azure/data-factory/connector-office-365)
- [Политики и выставление счетов](data-connect-policies.md)
